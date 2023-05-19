# Comparing `tmp/atproto-0.0.5.tar.gz` & `tmp/atproto-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atproto-0.0.5.tar", max compression
+gzip compressed data, was "atproto-0.0.6.tar", max compression
```

## Comparing `atproto-0.0.5.tar` & `atproto-0.0.6.tar`

### file list

```diff
@@ -1,167 +1,170 @@
--rw-r--r--   0        0        0     1061 2023-05-17 07:30:57.252256 atproto-0.0.5/LICENSE
--rw-r--r--   0        0        0     9596 2023-05-17 07:30:57.252256 atproto-0.0.5/README.md
--rw-r--r--   0        0        0      332 2023-05-17 07:30:57.252256 atproto-0.0.5/atproto/__init__.py
--rw-r--r--   0        0        0     1764 2023-05-17 07:30:57.252256 atproto-0.0.5/atproto/car/__init__.py
--rw-r--r--   0        0        0      137 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/cid/__init__.py
--rw-r--r--   0        0        0       23 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/cli/__init__.py
--rw-r--r--   0        0        0     2767 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/clients/__init__.py
--rw-r--r--   0        0        0     1156 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/clients/generate_async_client.py
--rw-r--r--   0        0        0        0 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/models/__init__.py
--rw-r--r--   0        0        0     2353 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/models/builder.py
--rw-r--r--   0        0        0    19303 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/models/generator.py
--rw-r--r--   0        0        0        0 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/namespaces/__init__.py
--rw-r--r--   0        0        0     2562 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/namespaces/builder.py
--rw-r--r--   0        0        0    11855 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/codegen/namespaces/generator.py
--rw-r--r--   0        0        0      944 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/exceptions.py
--rw-r--r--   0        0        0     2569 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/leb128/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/lexicon/__init__.py
--rw-r--r--   0        0        0     4658 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/lexicon/models.py
--rw-r--r--   0        0        0     3871 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/lexicon/parser.py
--rw-r--r--   0        0        0     5298 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/nsid/__init__.py
--rw-r--r--   0        0        0     3075 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/uri/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/client/__init__.py
--rw-r--r--   0        0        0     5994 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/client/async_client.py
--rw-r--r--   0        0        0      489 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/client/async_raw.py
--rw-r--r--   0        0        0     3719 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/client/base.py
--rw-r--r--   0        0        0     5555 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/client/client.py
--rw-r--r--   0        0        0      469 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/client/raw.py
--rw-r--r--   0        0        0    11424 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/__init__.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/__init__.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/__init__.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     4054 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      820 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py
--rw-r--r--   0        0        0      836 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      890 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0     1014 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      927 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/profile.py
--rw-r--r--   0        0        0      670 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py
--rw-r--r--   0        0        0     1061 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      970 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1778 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1564 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2457 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/record.py
--rw-r--r--   0        0        0     1248 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     4321 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/defs.py
--rw-r--r--   0        0        0     1041 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0     1497 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0     1076 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      855 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0     1181 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0     1066 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      734 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2441 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/post.py
--rw-r--r--   0        0        0      738 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/repost.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      665 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/block.py
--rw-r--r--   0        0        0     2446 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/defs.py
--rw-r--r--   0        0        0      667 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/follow.py
--rw-r--r--   0        0        0     1004 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0     1133 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0     1123 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0     1097 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_list.py
--rw-r--r--   0        0        0     1004 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py
--rw-r--r--   0        0        0     1033 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_lists.py
--rw-r--r--   0        0        0      999 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0     1121 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/list.py
--rw-r--r--   0        0        0      705 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/listitem.py
--rw-r--r--   0        0        0      574 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      575 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py
--rw-r--r--   0        0        0      576 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      577 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      830 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1932 2023-05-17 07:30:57.256256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      586 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0     1735 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0     1082 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      553 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/base.py
--rw-r--r--   0        0        0      713 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/blob_ref.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/__init__.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/__init__.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0    10100 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      595 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py
--rw-r--r--   0        0        0      712 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0      594 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py
--rw-r--r--   0        0        0     1071 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      839 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0     1097 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      839 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0     1231 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      890 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      824 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      953 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      911 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0     1129 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0     1370 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      651 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      621 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      887 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      586 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/defs.py
--rw-r--r--   0        0        0     1323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0     1077 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0     1499 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      825 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     2140 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0     1236 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      969 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0     1038 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0     1171 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1817 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1319 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      734 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py
--rw-r--r--   0        0        0      644 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      742 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_account.py
--rw-r--r--   0        0        0     1052 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      880 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0     1352 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0     1117 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1296 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/defs.py
--rw-r--r--   0        0        0      659 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0     1271 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0     1028 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      704 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/get_session.py
--rw-r--r--   0        0        0     1024 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      729 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      589 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      628 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      583 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0      323 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      752 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      744 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      822 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      986 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      764 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      872 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      916 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      969 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0     1253 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      637 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      640 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2782 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      547 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/type_conversion.py
--rw-r--r--   0        0        0     3285 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/models/utils.py
--rw-r--r--   0        0        0        0 2023-05-17 07:30:57.260256 atproto-0.0.5/atproto/xrpc_client/namespaces/__init__.py
--rw-r--r--   0        0        0    73381 2023-05-17 07:30:57.264256 atproto-0.0.5/atproto/xrpc_client/namespaces/async_ns.py
--rw-r--r--   0        0        0      361 2023-05-17 07:30:57.264256 atproto-0.0.5/atproto/xrpc_client/namespaces/base.py
--rw-r--r--   0        0        0    72323 2023-05-17 07:30:57.264256 atproto-0.0.5/atproto/xrpc_client/namespaces/sync_ns.py
--rw-r--r--   0        0        0     4353 2023-05-17 07:30:57.264256 atproto-0.0.5/atproto/xrpc_client/request.py
--rw-r--r--   0        0        0       43 2023-05-17 07:30:57.264256 atproto-0.0.5/atproto/xrpc_server/__init__.py
--rw-r--r--   0        0        0     2321 2023-05-17 07:31:29.892268 atproto-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    11450 1970-01-01 00:00:00.000000 atproto-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-19 21:17:17.186501 atproto-0.0.6/LICENSE
+-rw-r--r--   0        0        0     9588 2023-05-19 21:17:17.186501 atproto-0.0.6/README.md
+-rw-r--r--   0        0        0      332 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/__init__.py
+-rw-r--r--   0        0        0     1764 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/car/__init__.py
+-rw-r--r--   0        0        0      137 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/cid/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/cli/__init__.py
+-rw-r--r--   0        0        0     2767 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/clients/__init__.py
+-rw-r--r--   0        0        0     1319 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/clients/generate_async_client.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/models/__init__.py
+-rw-r--r--   0        0        0     2353 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/models/builder.py
+-rw-r--r--   0        0        0    19303 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/models/generator.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/namespaces/__init__.py
+-rw-r--r--   0        0        0     2562 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/namespaces/builder.py
+-rw-r--r--   0        0        0    11855 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/namespaces/generator.py
+-rw-r--r--   0        0        0      944 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/exceptions.py
+-rw-r--r--   0        0        0     2569 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/leb128/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/lexicon/__init__.py
+-rw-r--r--   0        0        0     4658 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/lexicon/models.py
+-rw-r--r--   0        0        0     3871 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/lexicon/parser.py
+-rw-r--r--   0        0        0     5298 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/nsid/__init__.py
+-rw-r--r--   0        0        0     3075 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/uri/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/__init__.py
+-rw-r--r--   0        0        0     7289 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/async_client.py
+-rw-r--r--   0        0        0      489 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/async_raw.py
+-rw-r--r--   0        0        0      421 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/auth.py
+-rw-r--r--   0        0        0     3719 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/base.py
+-rw-r--r--   0        0        0     6786 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/client.py
+-rw-r--r--   0        0        0       76 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/methods_mixin/__init__.py
+-rw-r--r--   0        0        0     1332 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/methods_mixin/session.py
+-rw-r--r--   0        0        0      469 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/raw.py
+-rw-r--r--   0        0        0    11424 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     4054 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      820 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py
+-rw-r--r--   0        0        0      836 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      890 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0     1014 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      927 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      670 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py
+-rw-r--r--   0        0        0     1061 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      970 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1778 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1564 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2457 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1248 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     4321 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0     1041 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0     1497 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0     1076 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      855 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0     1181 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0     1066 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      734 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2441 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      738 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      665 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/block.py
+-rw-r--r--   0        0        0     2446 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/defs.py
+-rw-r--r--   0        0        0      667 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0     1004 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0     1133 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0     1123 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0     1097 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_list.py
+-rw-r--r--   0        0        0     1004 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py
+-rw-r--r--   0        0        0     1033 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_lists.py
+-rw-r--r--   0        0        0      999 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0     1121 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/list.py
+-rw-r--r--   0        0        0      705 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/listitem.py
+-rw-r--r--   0        0        0      574 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      575 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py
+-rw-r--r--   0        0        0      576 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      577 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      830 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1932 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      586 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1735 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0     1082 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      553 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/base.py
+-rw-r--r--   0        0        0      713 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/blob_ref.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0    10850 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      595 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py
+-rw-r--r--   0        0        0      712 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      594 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py
+-rw-r--r--   0        0        0     1071 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      839 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0     1097 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      839 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0     1231 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      890 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      824 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      953 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      911 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0     1129 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1370 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      651 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      621 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      887 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      586 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/defs.py
+-rw-r--r--   0        0        0     1323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0     1077 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0     1499 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      825 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     2140 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0     1236 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      969 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0     1038 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0     1171 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1817 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1319 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      734 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py
+-rw-r--r--   0        0        0      644 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      742 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0     1052 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      880 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0     1352 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0     1117 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1296 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      659 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0     1271 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0     1028 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      704 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0     1024 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      729 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      589 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      628 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      583 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      752 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      744 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      822 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      986 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      764 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      872 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      916 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      969 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0     1253 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      637 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      640 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2782 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      547 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/type_conversion.py
+-rw-r--r--   0        0        0     3285 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/utils.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/namespaces/__init__.py
+-rw-r--r--   0        0        0    73381 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/namespaces/async_ns.py
+-rw-r--r--   0        0        0      361 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/namespaces/base.py
+-rw-r--r--   0        0        0    72323 2023-05-19 21:17:17.198502 atproto-0.0.6/atproto/xrpc_client/namespaces/sync_ns.py
+-rw-r--r--   0        0        0     4353 2023-05-19 21:17:17.198502 atproto-0.0.6/atproto/xrpc_client/request.py
+-rw-r--r--   0        0        0       43 2023-05-19 21:17:17.198502 atproto-0.0.6/atproto/xrpc_server/__init__.py
+-rw-r--r--   0        0        0     2396 2023-05-19 21:17:44.930884 atproto-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    11262 1970-01-01 00:00:00.000000 atproto-0.0.6/PKG-INFO
```

### Comparing `atproto-0.0.5/LICENSE` & `atproto-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/README.md` & `atproto-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     <br>
     <b>Autogenerated from lexicons, well type hinted, documented, sync and async SDK for Python</b>
     <br>
     <a href="https://github.com/MarshalX/atproto/tree/main/examples">
         Examples
     </a>
     •
-    <a href="https://atproto.rtfd.io">
+    <a href="https://atproto.blue">
         Documentation
     </a>
     •
     <a href="https://discord.gg/PCyVJXU9jN">
         Discord Bluesky API
     </a>
 </p>
@@ -133,15 +133,15 @@
 
 Useful links to continue:
 - [List of all methods with documentation](https://atproto.readthedocs.io/en/latest/xrpc_clients/client.html).
 - [Examples of using the methods](https://github.com/MarshalX/atproto/tree/main/examples).
 
 ### Documentation
 
-The documentation is live at [readthedocs.io](https://atproto.rtfd.io/).
+The documentation is live at [atproto.blue](https://atproto.blue/).
 
 ### Getting help
 
 You can get help in several ways:
 - Report bugs, request new features by [creating an issue](https://github.com/MarshalX/atproto/issues/new).
 - Ask questions by [starting a discussion](https://github.com/MarshalX/atproto/discussions/new).
 - Ask questions in [Discord server](https://discord.gg/ZDMSm3UGPN).
```

### Comparing `atproto-0.0.5/atproto/car/__init__.py` & `atproto-0.0.6/atproto/car/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/codegen/__init__.py` & `atproto-0.0.6/atproto/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/codegen/clients/generate_async_client.py` & `atproto-0.0.6/atproto/codegen/clients/generate_async_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,28 +9,32 @@
     with open(_CLIENT_DIR.joinpath(input_filename), 'r', encoding='UTF-8') as f:
         code = f.read()
 
     # TODO(MarshalX): Get automatically
     methods = [
         'send_post',
         'send_image',
+        '_get_and_set_session',
+        '_refresh_and_set_session',
+        '_invoke',
     ]
 
     code = code.replace('client.raw', 'client.async_raw')
     code = code.replace('class Client', 'class AsyncClient')
     code = code.replace('ClientRaw', 'AsyncClientRaw')
 
     code = code.replace('def', 'async def')
     code = code.replace('async def __', 'def __')
 
     code = code.replace('self.com', 'await self.com')
     code = code.replace('self.bsky', 'await self.bsky')
 
     for method in methods:
         code = code.replace(f'self.{method}', f'await self.{method}')
+        code = code.replace(f'super().{method}', f'await super().{method}')
 
     code = DISCLAIMER + code
 
     write_code(_CLIENT_DIR.joinpath(output_filename), code)
     format_code(_CLIENT_DIR.joinpath(output_filename))
```

### Comparing `atproto-0.0.5/atproto/codegen/models/builder.py` & `atproto-0.0.6/atproto/codegen/models/builder.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/codegen/models/generator.py` & `atproto-0.0.6/atproto/codegen/models/generator.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/codegen/namespaces/builder.py` & `atproto-0.0.6/atproto/codegen/namespaces/builder.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/codegen/namespaces/generator.py` & `atproto-0.0.6/atproto/codegen/namespaces/generator.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/exceptions.py` & `atproto-0.0.6/atproto/exceptions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/leb128/__init__.py` & `atproto-0.0.6/atproto/leb128/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/lexicon/models.py` & `atproto-0.0.6/atproto/lexicon/models.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/lexicon/parser.py` & `atproto-0.0.6/atproto/lexicon/parser.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/nsid/__init__.py` & `atproto-0.0.6/atproto/nsid/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/uri/__init__.py` & `atproto-0.0.6/atproto/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/client/async_client.py` & `atproto-0.0.6/atproto/xrpc_client/client/async_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,61 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 from datetime import datetime
-from typing import Optional, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.client.async_raw import AsyncClientRaw
+from atproto.xrpc_client.client.methods_mixin import SessionMethodsMixin
 
+if TYPE_CHECKING:
+    from atproto.xrpc_client.client.auth import JwtPayload
+    from atproto.xrpc_client.client.base import InvokeType
+    from atproto.xrpc_client.request import Response
 
-class AsyncClient(AsyncClientRaw):
+
+class AsyncClient(AsyncClientRaw, SessionMethodsMixin):
     """High-level client for XRPC of ATProto."""
 
     def __init__(self, base_url: str = None):
         super().__init__(base_url)
-        self.me = None
+
+        self._access_jwt: Optional[str] = None
+        self._access_jwt_payload: Optional['JwtPayload'] = None
+
+        self._refresh_jwt: Optional[str] = None
+        self._refresh_jwt_payload: Optional['JwtPayload'] = None
+
+        self.me: Optional[models.AppBskyActorDefs.ProfileViewDetailed] = None
+
+    async def _invoke(self, invoke_type: 'InvokeType', **kwargs) -> 'Response':
+        if self.me and self._should_refresh_session():
+            await self._refresh_and_set_session()
+
+        return await super()._invoke(invoke_type, **kwargs)
+
+    async def _get_and_set_session(self, login: str, password: str) -> models.ComAtprotoServerCreateSession.Response:
+        session = await self.com.atproto.server.create_session(
+            models.ComAtprotoServerCreateSession.Data(login, password)
+        )
+        self._set_session(session)
+
+        return session
+
+    async def _refresh_and_set_session(self) -> models.ComAtprotoServerRefreshSession.Response:
+        refresh_session = await self.com.atproto.server.refresh_session(
+            headers=self._get_auth_headers(self._refresh_jwt)
+        )
+        self._set_session(refresh_session)
+
+        return refresh_session
 
     async def login(self, login: str, password: str) -> models.AppBskyActorGetProfile.ResponseRef:
         """Authorize client and get profile info.
 
         Args:
             login: Handle/username of the account.
             password: Password of the account. Could be app specific one.
@@ -28,19 +63,15 @@
         Returns:
             :obj:`models.AppBskyActorGetProfile.ResponseRef`: Profile information.
 
         Raises:
             :class:`atproto.exceptions.AtProtocolError`: Base exception.
         """
 
-        session = await self.com.atproto.server.create_session(
-            models.ComAtprotoServerCreateSession.Data(login, password)
-        )
-        self.request.set_additional_headers({'Authorization': f'Bearer {session.accessJwt}'})
-
+        session = await self._get_and_set_session(login, password)
         self.me = await self.bsky.actor.get_profile(models.AppBskyActorGetProfile.Params(session.handle))
 
         return self.me
 
     async def send_post(
         self,
         text: str,
```

### Comparing `atproto-0.0.5/atproto/xrpc_client/client/base.py` & `atproto-0.0.6/atproto/xrpc_client/client/base.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/client/client.py` & `atproto-0.0.6/atproto/xrpc_client/client/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,51 @@
 from datetime import datetime
-from typing import Optional, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 from atproto.xrpc_client import models
+from atproto.xrpc_client.client.methods_mixin import SessionMethodsMixin
 from atproto.xrpc_client.client.raw import ClientRaw
 
+if TYPE_CHECKING:
+    from atproto.xrpc_client.client.auth import JwtPayload
+    from atproto.xrpc_client.client.base import InvokeType
+    from atproto.xrpc_client.request import Response
 
-class Client(ClientRaw):
+
+class Client(ClientRaw, SessionMethodsMixin):
     """High-level client for XRPC of ATProto."""
 
     def __init__(self, base_url: str = None):
         super().__init__(base_url)
-        self.me = None
+
+        self._access_jwt: Optional[str] = None
+        self._access_jwt_payload: Optional['JwtPayload'] = None
+
+        self._refresh_jwt: Optional[str] = None
+        self._refresh_jwt_payload: Optional['JwtPayload'] = None
+
+        self.me: Optional[models.AppBskyActorDefs.ProfileViewDetailed] = None
+
+    def _invoke(self, invoke_type: 'InvokeType', **kwargs) -> 'Response':
+        if self.me and self._should_refresh_session():
+            self._refresh_and_set_session()
+
+        return super()._invoke(invoke_type, **kwargs)
+
+    def _get_and_set_session(self, login: str, password: str) -> models.ComAtprotoServerCreateSession.Response:
+        session = self.com.atproto.server.create_session(models.ComAtprotoServerCreateSession.Data(login, password))
+        self._set_session(session)
+
+        return session
+
+    def _refresh_and_set_session(self) -> models.ComAtprotoServerRefreshSession.Response:
+        refresh_session = self.com.atproto.server.refresh_session(headers=self._get_auth_headers(self._refresh_jwt))
+        self._set_session(refresh_session)
+
+        return refresh_session
 
     def login(self, login: str, password: str) -> models.AppBskyActorGetProfile.ResponseRef:
         """Authorize client and get profile info.
 
         Args:
             login: Handle/username of the account.
             password: Password of the account. Could be app specific one.
@@ -22,17 +53,15 @@
         Returns:
             :obj:`models.AppBskyActorGetProfile.ResponseRef`: Profile information.
 
         Raises:
             :class:`atproto.exceptions.AtProtocolError`: Base exception.
         """
 
-        session = self.com.atproto.server.create_session(models.ComAtprotoServerCreateSession.Data(login, password))
-        self.request.set_additional_headers({'Authorization': f'Bearer {session.accessJwt}'})
-
+        session = self._get_and_set_session(login, password)
         self.me = self.bsky.actor.get_profile(models.AppBskyActorGetProfile.Params(session.handle))
 
         return self.me
 
     def send_post(
         self,
         text: str,
```

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/__init__.py` & `atproto-0.0.6/atproto/xrpc_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/defs.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_profile.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_profile.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/profile.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/profile.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/search_actors.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/search_actors.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/external.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/external.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/images.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/images.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/record.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/defs.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_likes.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_likes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_posts.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_posts.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/like.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/like.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/post.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/post.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/feed/repost.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/repost.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/block.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/block.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/defs.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/follow.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/follow.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_followers.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_followers.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_follows.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_follows.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_list.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_list.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_lists.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_lists.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/list.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/list.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/listitem.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/listitem.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/notification/update_seen.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/update_seen.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/richtext/facet.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/richtext/facet.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py` & `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/base.py` & `atproto-0.0.6/atproto/xrpc_client/models/base.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/blob_ref.py` & `atproto-0.0.6/atproto/xrpc_client/models/blob_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/defs.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,21 @@
 
     action: 'models.ComAtprotoAdminDefs.ActionType'
     createdAt: str
     createdBy: str
     id: int
     reason: str
     resolvedReports: List['models.ComAtprotoAdminDefs.ReportView']
-    subject: Union['models.ComAtprotoAdminDefs.RepoView', 'models.ComAtprotoAdminDefs.RecordView', 'Dict[str, Any]']
+    subject: Union[
+        'models.ComAtprotoAdminDefs.RepoView',
+        'models.ComAtprotoAdminDefs.RepoViewNotFound',
+        'models.ComAtprotoAdminDefs.RecordView',
+        'models.ComAtprotoAdminDefs.RecordViewNotFound',
+        'Dict[str, Any]',
+    ]
     subjectBlobs: List['models.ComAtprotoAdminDefs.BlobView']
     createLabelVals: Optional[List[str]] = None
     negateLabelVals: Optional[List[str]] = None
     reversal: Optional['models.ComAtprotoAdminDefs.ActionReversal'] = None
 
     _type: str = 'com.atproto.admin.defs#actionViewDetail'
 
@@ -169,15 +175,21 @@
     """
 
     createdAt: str
     id: int
     reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
     reportedBy: str
     resolvedByActions: List['models.ComAtprotoAdminDefs.ActionView']
-    subject: Union['models.ComAtprotoAdminDefs.RepoView', 'models.ComAtprotoAdminDefs.RecordView', 'Dict[str, Any]']
+    subject: Union[
+        'models.ComAtprotoAdminDefs.RepoView',
+        'models.ComAtprotoAdminDefs.RepoViewNotFound',
+        'models.ComAtprotoAdminDefs.RecordView',
+        'models.ComAtprotoAdminDefs.RecordViewNotFound',
+        'Dict[str, Any]',
+    ]
     reason: Optional[str] = None
 
     _type: str = 'com.atproto.admin.defs#reportViewDetail'
 
 
 @dataclass
 class RepoView(base.ModelBase):
@@ -236,14 +248,28 @@
     invitesDisabled: Optional[bool] = None
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
 
     _type: str = 'com.atproto.admin.defs#repoViewDetail'
 
 
 @dataclass
+class RepoViewNotFound(base.ModelBase):
+
+    """Definition model for :obj:`com.atproto.admin.defs`.
+
+    Attributes:
+        did: Did.
+    """
+
+    did: str
+
+    _type: str = 'com.atproto.admin.defs#repoViewNotFound'
+
+
+@dataclass
 class RepoRef(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
         did: Did.
     """
@@ -304,14 +330,28 @@
     value: 'base.RecordModelBase'
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
 
     _type: str = 'com.atproto.admin.defs#recordViewDetail'
 
 
 @dataclass
+class RecordViewNotFound(base.ModelBase):
+
+    """Definition model for :obj:`com.atproto.admin.defs`.
+
+    Attributes:
+        uri: Uri.
+    """
+
+    uri: str
+
+    _type: str = 'com.atproto.admin.defs#recordViewNotFound'
+
+
+@dataclass
 class Moderation(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
         currentAction: Current action.
     """
```

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_record.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/get_repo.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/search_repos.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/search_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/identity/update_handle.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/identity/update_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/defs.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/query_labels.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/query_labels.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/moderation/create_report.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/moderation/create_report.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/moderation/defs.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/moderation/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/create_record.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/create_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/delete_record.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/delete_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/get_record.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/list_records.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/list_records.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/put_record.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/put_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_account.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_account.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_app_password.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_app_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/create_session.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/defs.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/delete_account.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/delete_account.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/describe_server.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/describe_server.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/get_session.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/get_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/refresh_session.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/refresh_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/reset_password.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/reset_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_blob.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_blob.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_head.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_head.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_record.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/get_repo.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/list_repos.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/list_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py` & `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/type_conversion.py` & `atproto-0.0.6/atproto/xrpc_client/models/type_conversion.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/models/utils.py` & `atproto-0.0.6/atproto/xrpc_client/models/utils.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/namespaces/async_ns.py` & `atproto-0.0.6/atproto/xrpc_client/namespaces/async_ns.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/namespaces/sync_ns.py` & `atproto-0.0.6/atproto/xrpc_client/namespaces/sync_ns.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/atproto/xrpc_client/request.py` & `atproto-0.0.6/atproto/xrpc_client/request.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.5/pyproject.toml` & `atproto-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atproto"
-version = "0.0.5" # placeholder. Dynamic version from Git Tag
+version = "0.0.6" # placeholder. Dynamic version from Git Tag
 description = "The AT Protocol SDK"
 authors = ["Ilya (Marshal) <ilya@marshal.dev>"]
 license = "MIT"
 repository = "https://github.com/MarshalX/atproto"
 readme = "README.md"
 keywords = ["library", "sdk", "codegen", "xrpc", "xrpc-client", "atprotocol", "atproto", "lexicon", "parser", "schema", "bluesky", "bluesky-api", "at", "uri", "atp", "nsid", "did", "cid"]
 classifiers = [
@@ -23,25 +23,26 @@
 #    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Pre-processors",
 ]
 
 [tool.poetry.urls]
-"Documentation" = "https://atproto.rtfd.io"
+"Documentation" = "https://atproto.blue"
 "Author" = "https://github.com/MarshalX"
 "Tracker" = "https://github.com/MarshalX/atproto/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-httpx = "0.24.0"
-dacite = "1.8.0"
-multiformats = "0.2.1"
-typing-extensions = "4.5.0"
-dag-cbor = "0.3.2"
+python = ">=3.7,<3.12"
+httpx = ">=0.24.0,<0.25.0"
+dacite = ">=1.8.0,<1.9.0"
+multiformats = ">=0.2.1,<0.3.0"
+typing-extensions = ">=4.5.0,<4.6.0"
+dag-cbor = ">=0.3.2,<0.4.0"
+pyjwt = ">=2.7.0,<2.8.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 isort = "5.11.5"
 sphinx = "5.3.0"
```

### Comparing `atproto-0.0.5/PKG-INFO` & `atproto-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 Metadata-Version: 2.1
 Name: atproto
-Version: 0.0.5
+Version: 0.0.6
 Summary: The AT Protocol SDK
 Home-page: https://github.com/MarshalX/atproto
 License: MIT
 Keywords: library,sdk,codegen,xrpc,xrpc-client,atprotocol,atproto,lexicon,parser,schema,bluesky,bluesky-api,at,uri,atp,nsid,did,cid
 Author: Ilya (Marshal)
 Author-email: ilya@marshal.dev
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Pre-processors
-Requires-Dist: dacite (==1.8.0)
-Requires-Dist: dag-cbor (==0.3.2)
-Requires-Dist: httpx (==0.24.0)
-Requires-Dist: multiformats (==0.2.1)
-Requires-Dist: typing-extensions (==4.5.0)
+Requires-Dist: dacite (>=1.8.0,<1.9.0)
+Requires-Dist: dag-cbor (>=0.3.2,<0.4.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: multiformats (>=0.2.1,<0.3.0)
+Requires-Dist: pyjwt (>=2.7.0,<2.8.0)
+Requires-Dist: typing-extensions (>=4.5.0,<4.6.0)
 Project-URL: Author, https://github.com/MarshalX
-Project-URL: Documentation, https://atproto.rtfd.io
+Project-URL: Documentation, https://atproto.blue
 Project-URL: Repository, https://github.com/MarshalX/atproto
 Project-URL: Tracker, https://github.com/MarshalX/atproto/issues
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://github.com/MarshalX/atproto">
         <img alt="Logo of atproto SDK for Python by Midjourney'" src="https://github.com/MarshalX/atproto/raw/main/.github/images/logo.png">
@@ -47,15 +43,15 @@
     <br>
     <b>Autogenerated from lexicons, well type hinted, documented, sync and async SDK for Python</b>
     <br>
     <a href="https://github.com/MarshalX/atproto/tree/main/examples">
         Examples
     </a>
     •
-    <a href="https://atproto.rtfd.io">
+    <a href="https://atproto.blue">
         Documentation
     </a>
     •
     <a href="https://discord.gg/PCyVJXU9jN">
         Discord Bluesky API
     </a>
 </p>
@@ -175,15 +171,15 @@
 
 Useful links to continue:
 - [List of all methods with documentation](https://atproto.readthedocs.io/en/latest/xrpc_clients/client.html).
 - [Examples of using the methods](https://github.com/MarshalX/atproto/tree/main/examples).
 
 ### Documentation
 
-The documentation is live at [readthedocs.io](https://atproto.rtfd.io/).
+The documentation is live at [atproto.blue](https://atproto.blue/).
 
 ### Getting help
 
 You can get help in several ways:
 - Report bugs, request new features by [creating an issue](https://github.com/MarshalX/atproto/issues/new).
 - Ask questions by [starting a discussion](https://github.com/MarshalX/atproto/discussions/new).
 - Ask questions in [Discord server](https://discord.gg/ZDMSm3UGPN).
```

