# Comparing `tmp/twitter_api_py-0.7.1.tar.gz` & `tmp/twitter_api_py-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter_api_py-0.7.1.tar", max compression
+gzip compressed data, was "twitter_api_py-0.7.2.tar", max compression
```

## Comparing `twitter_api_py-0.7.1.tar` & `twitter_api_py-0.7.2.tar`

### file list

```diff
@@ -1,275 +1,275 @@
--rw-r--r--   0        0        0     1497 2023-05-15 17:02:23.490556 twitter_api_py-0.7.1/LICENSE
--rw-r--r--   0        0        0     2126 2023-05-15 17:02:23.490556 twitter_api_py-0.7.1/README.md
--rw-r--r--   0        0        0     1677 2023-05-15 17:02:23.522560 twitter_api_py-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      480 2023-05-15 17:02:23.542562 twitter_api_py-0.7.1/twitter_api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.542562 twitter_api_py-0.7.1/twitter_api/client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.542562 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/__init__.py
--rw-r--r--   0        0        0     1041 2023-05-15 17:02:23.542562 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
--rw-r--r--   0        0        0      311 2023-05-15 17:02:23.542562 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
--rw-r--r--   0        0        0      311 2023-05-15 17:02:23.542562 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth1_access_token_real_client.py
--rw-r--r--   0        0        0     1388 2023-05-15 17:02:23.542562 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
--rw-r--r--   0        0        0      306 2023-05-15 17:02:23.542562 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
--rw-r--r--   0        0        0      808 2023-05-15 17:02:23.542562 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
--rw-r--r--   0        0        0      315 2023-05-15 17:02:23.542562 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
--rw-r--r--   0        0        0      315 2023-05-15 17:02:23.542562 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth1_request_token_real_client.py
--rw-r--r--   0        0        0     1211 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
--rw-r--r--   0        0        0      311 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
--rw-r--r--   0        0        0      311 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth2_access_token_real_client.py
--rw-r--r--   0        0        0      831 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
--rw-r--r--   0        0        0      306 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
--rw-r--r--   0        0        0      306 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth2_authorization_real_client.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/__init__.py
--rw-r--r--   0        0        0      365 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
--rw-r--r--   0        0        0     1140 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
--rw-r--r--   0        0        0      462 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
--rw-r--r--   0        0        0      793 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
--rw-r--r--   0        0        0      444 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
--rw-r--r--   0        0        0      722 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
--rw-r--r--   0        0        0      392 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
--rw-r--r--   0        0        0      798 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
--rw-r--r--   0        0        0      501 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
--rw-r--r--   0        0        0      751 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
--rw-r--r--   0        0        0      648 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/session_resources.py
--rw-r--r--   0        0        0      357 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
--rw-r--r--   0        0        0     1596 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
--rw-r--r--   0        0        0     1875 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
--rw-r--r--   0        0        0     4005 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
--rw-r--r--   0        0        0     1103 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/twitter_oauth1_session.py
--rw-r--r--   0        0        0     1716 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
--rw-r--r--   0        0        0     3466 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
--rw-r--r--   0        0        0      823 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/oauth_session/twitter_oauth2_session.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/request/__init__.py
--rw-r--r--   0        0        0     1375 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/request/request_async_client.py
--rw-r--r--   0        0        0      458 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/request/request_async_mock_client.py
--rw-r--r--   0        0        0     5306 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/request/request_async_real_client.py
--rw-r--r--   0        0        0     1786 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/request/request_client.py
--rw-r--r--   0        0        0     3673 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/request/request_mock_client.py
--rw-r--r--   0        0        0     7358 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/request/request_real_client.py
--rw-r--r--   0        0        0    32159 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/twitter_api_async_client.py
--rw-r--r--   0        0        0    14922 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/twitter_api_async_mock_client.py
--rw-r--r--   0        0        0    14633 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/twitter_api_async_real_client.py
--rw-r--r--   0        0        0    31932 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/twitter_api_client.py
--rw-r--r--   0        0        0    27278 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/twitter_api_mock_client.py
--rw-r--r--   0        0        0    13624 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/client/twitter_api_real_client.py
--rw-r--r--   0        0        0    10801 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/error.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/__init__.py
--rw-r--r--   0        0        0      603 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/manager/__init__.py
--rw-r--r--   0        0        0      677 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
--rw-r--r--   0        0        0     1301 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/manager/mixins/__init__.py
--rw-r--r--   0        0        0     2251 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/manager/mixins/dict_rate_limit_checker_mixin.py
--rw-r--r--   0        0        0      672 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/manager/mixins/raise_rate_limit_handler_mixin.py
--rw-r--r--   0        0        0     3287 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/manager/mixins/sleep_rate_limit_handler_mixin.py
--rw-r--r--   0        0        0      908 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
--rw-r--r--   0        0        0     1358 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/manager/rate_limit_manager.py
--rw-r--r--   0        0        0     3751 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/rate_limit.py
--rw-r--r--   0        0        0      291 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/rate_limit_info.py
--rw-r--r--   0        0        0      102 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/rate_limit/rate_limit_target.py
--rw-r--r--   0        0        0      281 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/api_resources.py
--rw-r--r--   0        0        0      437 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/oauth2_invalidate_token/__init__.py
--rw-r--r--   0        0        0     2331 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
--rw-r--r--   0        0        0      332 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/oauth2_token/__init__.py
--rw-r--r--   0        0        0     2223 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/oauth2_token/post_oauth2_token.py
--rw-r--r--   0        0        0      522 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversation_messages/__init__.py
--rw-r--r--   0        0        0     2370 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
--rw-r--r--   0        0        0      422 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversations/__init__.py
--rw-r--r--   0        0        0     2199 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py
--rw-r--r--   0        0        0      654 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
--rw-r--r--   0        0        0     8948 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
--rw-r--r--   0        0        0      657 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py
--rw-r--r--   0        0        0     2444 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
--rw-r--r--   0        0        0      429 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweet/__init__.py
--rw-r--r--   0        0        0     1492 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweet/delete_v2_tweet.py
--rw-r--r--   0        0        0     3142 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweet/get_v2_tweet.py
--rw-r--r--   0        0        0      439 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweet_retweeted_by/__init__.py
--rw-r--r--   0        0        0     6602 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
--rw-r--r--   0        0        0      428 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweets/__init__.py
--rw-r--r--   0        0        0     3007 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweets/get_v2_tweets.py
--rw-r--r--   0        0        0     2956 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweets/post_v2_tweets.py
--rw-r--r--   0        0        0      419 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_all/__init__.py
--rw-r--r--   0        0        0     6019 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
--rw-r--r--   0        0        0      452 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_recent/__init__.py
--rw-r--r--   0        0        0     6118 2023-05-15 17:02:23.546563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
--rw-r--r--   0        0        0      452 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_stream/__init__.py
--rw-r--r--   0        0        0     3669 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
--rw-r--r--   0        0        0      751 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py
--rw-r--r--   0        0        0     2164 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0     3149 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0      286 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_user/__init__.py
--rw-r--r--   0        0        0     2833 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_user/get_v2_user.py
--rw-r--r--   0        0        0      382 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_user_followers/__init__.py
--rw-r--r--   0        0        0     6551 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_user_followers/get_v2_user_followers.py
--rw-r--r--   0        0        0      387 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_user_following/__init__.py
--rw-r--r--   0        0        0     1944 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_user_following/post_v2_user_following.py
--rw-r--r--   0        0        0      402 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_user_liked_tweets/__init__.py
--rw-r--r--   0        0        0     7972 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
--rw-r--r--   0        0        0      378 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_user_retweets/__init__.py
--rw-r--r--   0        0        0     1946 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py
--rw-r--r--   0        0        0      342 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_user_tweets/__init__.py
--rw-r--r--   0        0        0     8381 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py
--rw-r--r--   0        0        0      290 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_users/__init__.py
--rw-r--r--   0        0        0     2733 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_users/get_v2_users.py
--rw-r--r--   0        0        0      310 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_users_by/__init__.py
--rw-r--r--   0        0        0     2808 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_users_by/get_v2_users_by.py
--rw-r--r--   0        0        0      407 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_users_by_username/__init__.py
--rw-r--r--   0        0        0     3078 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/__init__.py
--rw-r--r--   0        0        0      397 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/_chainable.py
--rw-r--r--   0        0        0      858 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/_generic_client.py
--rw-r--r--   0        0        0     2362 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/_model.py
--rw-r--r--   0        0        0     3413 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/_paging.py
--rw-r--r--   0        0        0      727 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/comma_separatable.py
--rw-r--r--   0        0        0      246 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/endpoint.py
--rw-r--r--   0        0        0     1581 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/extra_permissive_model.py
--rw-r--r--   0        0        0      645 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/http.py
--rw-r--r--   0        0        0      744 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/httpx.py
--rw-r--r--   0        0        0     1971 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/oauth.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/oauth1/__init__.py
--rw-r--r--   0        0        0     2037 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/oauth1/oauth1_access_token.py
--rw-r--r--   0        0        0     3474 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/oauth1/oauth1_authorization.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/oauth2/__init__.py
--rw-r--r--   0        0        0     1975 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/oauth2/oauth2_access_token.py
--rw-r--r--   0        0        0     3593 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/oauth2/oauth2_authorization.py
--rw-r--r--   0        0        0       74 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/pagination_token.py
--rw-r--r--   0        0        0       66 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_cashtag.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_dm_conversation/__init__.py
--rw-r--r--   0        0        0      337 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_dm_conversation/dm_conversation.py
--rw-r--r--   0        0        0      212 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_dm_conversation/dm_conversation_attachment.py
--rw-r--r--   0        0        0       75 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_dm_conversation/dm_conversation_id.py
--rw-r--r--   0        0        0      624 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_dm_conversation/dm_conversation_message.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_dm_event/__init__.py
--rw-r--r--   0        0        0      342 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_dm_event/dm_event_expansion.py
--rw-r--r--   0        0        0      448 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_dm_event/dm_event_field.py
--rw-r--r--   0        0        0       68 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_dm_event/dm_event_id.py
--rw-r--r--   0        0        0      249 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_dm_event/dm_event_type.py
--rw-r--r--   0        0        0      368 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_domain.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_entity/__init__.py
--rw-r--r--   0        0        0      286 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_entity/entity.py
--rw-r--r--   0        0        0       67 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_entity/entity_id.py
--rw-r--r--   0        0        0       69 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_entity/entity_name.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_geo/__init__.py
--rw-r--r--   0        0        0      220 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_geo/geo.py
--rw-r--r--   0        0        0       66 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_hashtag.py
--rw-r--r--   0        0        0      773 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_language.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_list/__init__.py
--rw-r--r--   0        0        0       65 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_list/list_id.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_media/__init__.py
--rw-r--r--   0        0        0     1386 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_media/media.py
--rw-r--r--   0        0        0      581 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_media/media_field.py
--rw-r--r--   0        0        0      111 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_media/media_id.py
--rw-r--r--   0        0        0       67 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_media/media_key.py
--rw-r--r--   0        0        0      376 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_media/media_non_public_metrics.py
--rw-r--r--   0        0        0      411 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_media/media_organic_metrics.py
--rw-r--r--   0        0        0      412 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_media/media_promoted_metrics.py
--rw-r--r--   0        0        0      190 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_media/media_public_metrics.py
--rw-r--r--   0        0        0      211 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_media/media_variants.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_place/__init__.py
--rw-r--r--   0        0        0      933 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_place/place.py
--rw-r--r--   0        0        0     2723 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_place/place_country_code.py
--rw-r--r--   0        0        0      359 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_place/place_field.py
--rw-r--r--   0        0        0       72 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_place/place_full_name.py
--rw-r--r--   0        0        0      105 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_place/place_id.py
--rw-r--r--   0        0        0       68 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_place/place_name.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_poll/__init__.py
--rw-r--r--   0        0        0      593 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_poll/poll.py
--rw-r--r--   0        0        0      283 2023-05-15 17:02:23.550563 twitter_api_py-0.7.1/twitter_api/types/v2_poll/poll_field.py
--rw-r--r--   0        0        0       65 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_poll/poll_id.py
--rw-r--r--   0        0        0      164 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_poll/poll_option.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_retweet/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet.py
--rw-r--r--   0        0        0      392 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet_entities.py
--rw-r--r--   0        0        0      913 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet_entities_description.py
--rw-r--r--   0        0        0      237 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet_entities_description_cashtag.py
--rw-r--r--   0        0        0      237 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet_entities_description_hashtag.py
--rw-r--r--   0        0        0      246 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet_entities_description_mention.py
--rw-r--r--   0        0        0      258 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet_entities_description_url.py
--rw-r--r--   0        0        0      338 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet_entities_url.py
--rw-r--r--   0        0        0      254 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet_includes.py
--rw-r--r--   0        0        0      219 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet_public_metrics.py
--rw-r--r--   0        0        0      382 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet_withheld.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_rule/__init__.py
--rw-r--r--   0        0        0      311 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_rule/rule.py
--rw-r--r--   0        0        0       65 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_rule/rule_id.py
--rw-r--r--   0        0        0       66 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_rule/rule_tag.py
--rw-r--r--   0        0        0     1411 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_scope.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/__init__.py
--rw-r--r--   0        0        0      873 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/_and_operator.py
--rw-r--r--   0        0        0      305 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/_markable_operator.py
--rw-r--r--   0        0        0      521 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/_not_operator.py
--rw-r--r--   0        0        0      662 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/_or_operator.py
--rw-r--r--   0        0        0      700 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/bounding_box_operator.py
--rw-r--r--   0        0        0      339 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/cashtag_operator.py
--rw-r--r--   0        0        0     1361 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/context_operator.py
--rw-r--r--   0        0        0      380 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/conversation_id_operator.py
--rw-r--r--   0        0        0      341 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/entity_operator.py
--rw-r--r--   0        0        0      424 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/from_user_operator.py
--rw-r--r--   0        0        0     1547 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/group_operator.py
--rw-r--r--   0        0        0      219 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/has_cashtags_operator.py
--rw-r--r--   0        0        0      209 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/has_geo_operator.py
--rw-r--r--   0        0        0      219 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/has_hashtags_operator.py
--rw-r--r--   0        0        0      215 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/has_images_operator.py
--rw-r--r--   0        0        0      213 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/has_links_operator.py
--rw-r--r--   0        0        0      213 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/has_media_operator.py
--rw-r--r--   0        0        0      219 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/has_mentions_operator.py
--rw-r--r--   0        0        0      222 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/has_video_link_operator.py
--rw-r--r--   0        0        0      339 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/hashtag_operator.py
--rw-r--r--   0        0        0      349 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/in_reply_to_tweet_id_operator.py
--rw-r--r--   0        0        0      442 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/is_nullcast_operator.py
--rw-r--r--   0        0        0      211 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/is_quote_operator.py
--rw-r--r--   0        0        0      211 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/is_reply_operator.py
--rw-r--r--   0        0        0      215 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/is_retweet_operator.py
--rw-r--r--   0        0        0      217 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/is_verified_operator.py
--rw-r--r--   0        0        0      416 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/keyword_operator.py
--rw-r--r--   0        0        0      339 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/lang_operator.py
--rw-r--r--   0        0        0      317 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/list_operator.py
--rw-r--r--   0        0        0      349 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/mention_operator.py
--rw-r--r--   0        0        0     2648 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/operator.py
--rw-r--r--   0        0        0      370 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/place_country_operator.py
--rw-r--r--   0        0        0      544 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/place_operator.py
--rw-r--r--   0        0        0     1328 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/point_radius_operator.py
--rw-r--r--   0        0        0      354 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/quotes_of_tweet_id_operator.py
--rw-r--r--   0        0        0      433 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/retweets_of_operator.py
--rw-r--r--   0        0        0      350 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/retweets_of_tweet_id_operator.py
--rw-r--r--   0        0        0      420 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/to_user_operator.py
--rw-r--r--   0        0        0      262 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/url_operator.py
--rw-r--r--   0        0        0     2495 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/search_query.py
--rw-r--r--   0        0        0    14382 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_search_query/search_query_builder.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/__init__.py
--rw-r--r--   0        0        0     7856 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet.py
--rw-r--r--   0        0        0      309 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_attachments.py
--rw-r--r--   0        0        0      267 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_context_annotation.py
--rw-r--r--   0        0        0      314 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_edit_controls.py
--rw-r--r--   0        0        0      720 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_entities.py
--rw-r--r--   0        0        0      333 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_entities_annotation.py
--rw-r--r--   0        0        0      247 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_entities_cashtag.py
--rw-r--r--   0        0        0      247 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_entities_hashtag.py
--rw-r--r--   0        0        0      313 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_entities_mention.py
--rw-r--r--   0        0        0      415 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_entities_url.py
--rw-r--r--   0        0        0      643 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_expansion.py
--rw-r--r--   0        0        0     1921 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_field.py
--rw-r--r--   0        0        0      288 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_geo.py
--rw-r--r--   0        0        0      231 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_geo_coordinates.py
--rw-r--r--   0        0        0      111 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_id.py
--rw-r--r--   0        0        0      287 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_non_public_metrics.py
--rw-r--r--   0        0        0      285 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_organic_metrics.py
--rw-r--r--   0        0        0      286 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_promoted_metrics.py
--rw-r--r--   0        0        0      437 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_public_metrics.py
--rw-r--r--   0        0        0      267 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_referenced_tweet.py
--rw-r--r--   0        0        0     7079 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_response_body.py
--rw-r--r--   0        0        0      417 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_withheld.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_user/__init__.py
--rw-r--r--   0        0        0      969 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_user/user.py
--rw-r--r--   0        0        0      168 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_user/user_expantion.py
--rw-r--r--   0        0        0      619 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_user/user_field.py
--rw-r--r--   0        0        0       65 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_user/user_id.py
--rw-r--r--   0        0        0      108 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_user/user_verified_type.py
--rw-r--r--   0        0        0      139 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/types/v2_user/username.py
--rw-r--r--   0        0        0        0 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/utils/__init__.py
--rw-r--r--   0        0        0      123 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/utils/_datetime.py
--rw-r--r--   0        0        0      716 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/utils/_functional.py
--rw-r--r--   0        0        0      904 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/utils/_oauth.py
--rw-r--r--   0        0        0      790 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/utils/json.py
--rw-r--r--   0        0        0      630 2023-05-15 17:02:23.554563 twitter_api_py-0.7.1/twitter_api/warning.py
--rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 twitter_api_py-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-05-19 00:41:37.662857 twitter_api_py-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2126 2023-05-19 00:41:37.662857 twitter_api_py-0.7.2/README.md
+-rw-r--r--   0        0        0     1654 2023-05-19 00:41:37.698857 twitter_api_py-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      480 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/__init__.py
+-rw-r--r--   0        0        0     1041 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
+-rw-r--r--   0        0        0      311 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
+-rw-r--r--   0        0        0      311 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth1_access_token_real_client.py
+-rw-r--r--   0        0        0     1388 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
+-rw-r--r--   0        0        0      306 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
+-rw-r--r--   0        0        0      808 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
+-rw-r--r--   0        0        0      315 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
+-rw-r--r--   0        0        0      315 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth1_request_token_real_client.py
+-rw-r--r--   0        0        0     1211 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
+-rw-r--r--   0        0        0      311 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
+-rw-r--r--   0        0        0      311 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth2_access_token_real_client.py
+-rw-r--r--   0        0        0      831 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
+-rw-r--r--   0        0        0      306 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
+-rw-r--r--   0        0        0      306 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth2_authorization_real_client.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/__init__.py
+-rw-r--r--   0        0        0      365 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
+-rw-r--r--   0        0        0     1140 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
+-rw-r--r--   0        0        0      462 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
+-rw-r--r--   0        0        0      793 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
+-rw-r--r--   0        0        0      444 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
+-rw-r--r--   0        0        0      722 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
+-rw-r--r--   0        0        0      392 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
+-rw-r--r--   0        0        0      798 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
+-rw-r--r--   0        0        0      501 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
+-rw-r--r--   0        0        0      751 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
+-rw-r--r--   0        0        0      648 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/session_resources.py
+-rw-r--r--   0        0        0      357 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
+-rw-r--r--   0        0        0     1596 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
+-rw-r--r--   0        0        0     1875 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
+-rw-r--r--   0        0        0     4005 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
+-rw-r--r--   0        0        0     1103 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/twitter_oauth1_session.py
+-rw-r--r--   0        0        0     1716 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
+-rw-r--r--   0        0        0     3466 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
+-rw-r--r--   0        0        0      823 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/oauth_session/twitter_oauth2_session.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/request/__init__.py
+-rw-r--r--   0        0        0     1375 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/request/request_async_client.py
+-rw-r--r--   0        0        0      460 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/request/request_async_mock_client.py
+-rw-r--r--   0        0        0     5306 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/request/request_async_real_client.py
+-rw-r--r--   0        0        0     1786 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/request/request_client.py
+-rw-r--r--   0        0        0     3832 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/request/request_mock_client.py
+-rw-r--r--   0        0        0     7358 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/request/request_real_client.py
+-rw-r--r--   0        0        0    32384 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/twitter_api_async_client.py
+-rw-r--r--   0        0        0    15048 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/twitter_api_async_mock_client.py
+-rw-r--r--   0        0        0    14661 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/twitter_api_async_real_client.py
+-rw-r--r--   0        0        0    32143 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/twitter_api_client.py
+-rw-r--r--   0        0        0    27423 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/twitter_api_mock_client.py
+-rw-r--r--   0        0        0    13652 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/client/twitter_api_real_client.py
+-rw-r--r--   0        0        0    10984 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/error.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/__init__.py
+-rw-r--r--   0        0        0      603 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/manager/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
+-rw-r--r--   0        0        0     1301 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/manager/mixins/__init__.py
+-rw-r--r--   0        0        0     2251 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/manager/mixins/dict_rate_limit_checker_mixin.py
+-rw-r--r--   0        0        0      672 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/manager/mixins/raise_rate_limit_handler_mixin.py
+-rw-r--r--   0        0        0     3287 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/manager/mixins/sleep_rate_limit_handler_mixin.py
+-rw-r--r--   0        0        0      908 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
+-rw-r--r--   0        0        0     1358 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/manager/rate_limit_manager.py
+-rw-r--r--   0        0        0     3751 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/rate_limit.py
+-rw-r--r--   0        0        0      291 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/rate_limit_info.py
+-rw-r--r--   0        0        0      102 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/rate_limit/rate_limit_target.py
+-rw-r--r--   0        0        0      281 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/resources/api_resources.py
+-rw-r--r--   0        0        0      437 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/resources/oauth2_invalidate_token/__init__.py
+-rw-r--r--   0        0        0     2331 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
+-rw-r--r--   0        0        0      332 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/resources/oauth2_token/__init__.py
+-rw-r--r--   0        0        0     2223 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/resources/oauth2_token/post_oauth2_token.py
+-rw-r--r--   0        0        0      522 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversation_messages/__init__.py
+-rw-r--r--   0        0        0     2370 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
+-rw-r--r--   0        0        0      422 2023-05-19 00:41:37.718858 twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversations/__init__.py
+-rw-r--r--   0        0        0     2199 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py
+-rw-r--r--   0        0        0      654 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
+-rw-r--r--   0        0        0     8948 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
+-rw-r--r--   0        0        0      657 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py
+-rw-r--r--   0        0        0     2444 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
+-rw-r--r--   0        0        0      429 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     1492 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweet/delete_v2_tweet.py
+-rw-r--r--   0        0        0     3142 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweet/get_v2_tweet.py
+-rw-r--r--   0        0        0      439 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweet_retweeted_by/__init__.py
+-rw-r--r--   0        0        0     6602 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
+-rw-r--r--   0        0        0      428 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweets/__init__.py
+-rw-r--r--   0        0        0     3007 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweets/get_v2_tweets.py
+-rw-r--r--   0        0        0     2956 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweets/post_v2_tweets.py
+-rw-r--r--   0        0        0      419 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_all/__init__.py
+-rw-r--r--   0        0        0     6019 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
+-rw-r--r--   0        0        0      452 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_recent/__init__.py
+-rw-r--r--   0        0        0     6118 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
+-rw-r--r--   0        0        0      452 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_stream/__init__.py
+-rw-r--r--   0        0        0     3669 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
+-rw-r--r--   0        0        0      751 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py
+-rw-r--r--   0        0        0     2164 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0     3149 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0      286 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_user/__init__.py
+-rw-r--r--   0        0        0     2833 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_user/get_v2_user.py
+-rw-r--r--   0        0        0      382 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_user_followers/__init__.py
+-rw-r--r--   0        0        0     6551 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_user_followers/get_v2_user_followers.py
+-rw-r--r--   0        0        0      387 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_user_following/__init__.py
+-rw-r--r--   0        0        0     1944 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_user_following/post_v2_user_following.py
+-rw-r--r--   0        0        0      402 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_user_liked_tweets/__init__.py
+-rw-r--r--   0        0        0     7972 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
+-rw-r--r--   0        0        0      378 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_user_retweets/__init__.py
+-rw-r--r--   0        0        0     1946 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py
+-rw-r--r--   0        0        0      342 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_user_tweets/__init__.py
+-rw-r--r--   0        0        0     8381 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py
+-rw-r--r--   0        0        0      290 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_users/__init__.py
+-rw-r--r--   0        0        0     2733 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_users/get_v2_users.py
+-rw-r--r--   0        0        0      310 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_users_by/__init__.py
+-rw-r--r--   0        0        0     2808 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_users_by/get_v2_users_by.py
+-rw-r--r--   0        0        0      407 2023-05-19 00:41:37.722858 twitter_api_py-0.7.2/twitter_api/resources/v2_users_by_username/__init__.py
+-rw-r--r--   0        0        0     3078 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/_chainable.py
+-rw-r--r--   0        0        0      858 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/_generic_client.py
+-rw-r--r--   0        0        0     2362 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/_model.py
+-rw-r--r--   0        0        0     3413 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/_paging.py
+-rw-r--r--   0        0        0      727 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/comma_separatable.py
+-rw-r--r--   0        0        0      246 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/endpoint.py
+-rw-r--r--   0        0        0     1581 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/extra_permissive_model.py
+-rw-r--r--   0        0        0      645 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/http.py
+-rw-r--r--   0        0        0      744 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/httpx.py
+-rw-r--r--   0        0        0     1971 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/oauth.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/oauth1/__init__.py
+-rw-r--r--   0        0        0     2037 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/oauth1/oauth1_access_token.py
+-rw-r--r--   0        0        0     3474 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/oauth1/oauth1_authorization.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/oauth2/__init__.py
+-rw-r--r--   0        0        0     1975 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/oauth2/oauth2_access_token.py
+-rw-r--r--   0        0        0     3593 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/oauth2/oauth2_authorization.py
+-rw-r--r--   0        0        0       74 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/pagination_token.py
+-rw-r--r--   0        0        0       66 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_cashtag.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_dm_conversation/__init__.py
+-rw-r--r--   0        0        0      337 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_dm_conversation/dm_conversation.py
+-rw-r--r--   0        0        0      212 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_dm_conversation/dm_conversation_attachment.py
+-rw-r--r--   0        0        0       75 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_dm_conversation/dm_conversation_id.py
+-rw-r--r--   0        0        0      624 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_dm_conversation/dm_conversation_message.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_dm_event/__init__.py
+-rw-r--r--   0        0        0      342 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_dm_event/dm_event_expansion.py
+-rw-r--r--   0        0        0      448 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_dm_event/dm_event_field.py
+-rw-r--r--   0        0        0       68 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_dm_event/dm_event_id.py
+-rw-r--r--   0        0        0      249 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_dm_event/dm_event_type.py
+-rw-r--r--   0        0        0      368 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_domain.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_entity/__init__.py
+-rw-r--r--   0        0        0      286 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_entity/entity.py
+-rw-r--r--   0        0        0       67 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_entity/entity_id.py
+-rw-r--r--   0        0        0       69 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_entity/entity_name.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_geo/__init__.py
+-rw-r--r--   0        0        0      220 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_geo/geo.py
+-rw-r--r--   0        0        0       66 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_hashtag.py
+-rw-r--r--   0        0        0      773 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_language.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_list/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_list/list_id.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_media/__init__.py
+-rw-r--r--   0        0        0     1386 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_media/media.py
+-rw-r--r--   0        0        0      581 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_media/media_field.py
+-rw-r--r--   0        0        0      111 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_media/media_id.py
+-rw-r--r--   0        0        0       67 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_media/media_key.py
+-rw-r--r--   0        0        0      376 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_media/media_non_public_metrics.py
+-rw-r--r--   0        0        0      411 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_media/media_organic_metrics.py
+-rw-r--r--   0        0        0      412 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_media/media_promoted_metrics.py
+-rw-r--r--   0        0        0      190 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_media/media_public_metrics.py
+-rw-r--r--   0        0        0      211 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_media/media_variants.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_place/__init__.py
+-rw-r--r--   0        0        0      933 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_place/place.py
+-rw-r--r--   0        0        0     2723 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_place/place_country_code.py
+-rw-r--r--   0        0        0      359 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_place/place_field.py
+-rw-r--r--   0        0        0       72 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_place/place_full_name.py
+-rw-r--r--   0        0        0      105 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_place/place_id.py
+-rw-r--r--   0        0        0       68 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_place/place_name.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_poll/__init__.py
+-rw-r--r--   0        0        0      593 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_poll/poll.py
+-rw-r--r--   0        0        0      283 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_poll/poll_field.py
+-rw-r--r--   0        0        0       65 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_poll/poll_id.py
+-rw-r--r--   0        0        0      164 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_poll/poll_option.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_retweet/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet.py
+-rw-r--r--   0        0        0      392 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet_entities.py
+-rw-r--r--   0        0        0      913 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet_entities_description.py
+-rw-r--r--   0        0        0      237 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet_entities_description_cashtag.py
+-rw-r--r--   0        0        0      237 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet_entities_description_hashtag.py
+-rw-r--r--   0        0        0      246 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet_entities_description_mention.py
+-rw-r--r--   0        0        0      258 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet_entities_description_url.py
+-rw-r--r--   0        0        0      338 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet_entities_url.py
+-rw-r--r--   0        0        0      254 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet_includes.py
+-rw-r--r--   0        0        0      219 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet_public_metrics.py
+-rw-r--r--   0        0        0      382 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_rule/__init__.py
+-rw-r--r--   0        0        0      311 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_rule/rule.py
+-rw-r--r--   0        0        0       65 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_rule/rule_id.py
+-rw-r--r--   0        0        0       66 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_rule/rule_tag.py
+-rw-r--r--   0        0        0     1411 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_scope.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/__init__.py
+-rw-r--r--   0        0        0      873 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/_and_operator.py
+-rw-r--r--   0        0        0      305 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/_markable_operator.py
+-rw-r--r--   0        0        0      521 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/_not_operator.py
+-rw-r--r--   0        0        0      662 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/_or_operator.py
+-rw-r--r--   0        0        0      700 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/bounding_box_operator.py
+-rw-r--r--   0        0        0      339 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/cashtag_operator.py
+-rw-r--r--   0        0        0     1361 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/context_operator.py
+-rw-r--r--   0        0        0      380 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/conversation_id_operator.py
+-rw-r--r--   0        0        0      341 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/entity_operator.py
+-rw-r--r--   0        0        0      424 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/from_user_operator.py
+-rw-r--r--   0        0        0     1547 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/group_operator.py
+-rw-r--r--   0        0        0      219 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/has_cashtags_operator.py
+-rw-r--r--   0        0        0      209 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/has_geo_operator.py
+-rw-r--r--   0        0        0      219 2023-05-19 00:41:37.726858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/has_hashtags_operator.py
+-rw-r--r--   0        0        0      215 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/has_images_operator.py
+-rw-r--r--   0        0        0      213 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/has_links_operator.py
+-rw-r--r--   0        0        0      213 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/has_media_operator.py
+-rw-r--r--   0        0        0      219 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/has_mentions_operator.py
+-rw-r--r--   0        0        0      222 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/has_video_link_operator.py
+-rw-r--r--   0        0        0      339 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/hashtag_operator.py
+-rw-r--r--   0        0        0      349 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/in_reply_to_tweet_id_operator.py
+-rw-r--r--   0        0        0      442 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/is_nullcast_operator.py
+-rw-r--r--   0        0        0      211 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/is_quote_operator.py
+-rw-r--r--   0        0        0      211 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/is_reply_operator.py
+-rw-r--r--   0        0        0      215 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/is_retweet_operator.py
+-rw-r--r--   0        0        0      217 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/is_verified_operator.py
+-rw-r--r--   0        0        0      416 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/keyword_operator.py
+-rw-r--r--   0        0        0      339 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/lang_operator.py
+-rw-r--r--   0        0        0      317 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/list_operator.py
+-rw-r--r--   0        0        0      349 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/mention_operator.py
+-rw-r--r--   0        0        0     2670 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/operator.py
+-rw-r--r--   0        0        0      370 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/place_country_operator.py
+-rw-r--r--   0        0        0      544 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/place_operator.py
+-rw-r--r--   0        0        0     1328 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/point_radius_operator.py
+-rw-r--r--   0        0        0      354 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/quotes_of_tweet_id_operator.py
+-rw-r--r--   0        0        0      433 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/retweets_of_operator.py
+-rw-r--r--   0        0        0      350 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/retweets_of_tweet_id_operator.py
+-rw-r--r--   0        0        0      420 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/to_user_operator.py
+-rw-r--r--   0        0        0      262 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/url_operator.py
+-rw-r--r--   0        0        0     2495 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/search_query.py
+-rw-r--r--   0        0        0    14382 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_search_query/search_query_builder.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     7856 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet.py
+-rw-r--r--   0        0        0      309 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_attachments.py
+-rw-r--r--   0        0        0      267 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_context_annotation.py
+-rw-r--r--   0        0        0      314 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_edit_controls.py
+-rw-r--r--   0        0        0      720 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_entities.py
+-rw-r--r--   0        0        0      333 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_entities_annotation.py
+-rw-r--r--   0        0        0      247 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_entities_cashtag.py
+-rw-r--r--   0        0        0      247 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_entities_hashtag.py
+-rw-r--r--   0        0        0      313 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_entities_mention.py
+-rw-r--r--   0        0        0      415 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_entities_url.py
+-rw-r--r--   0        0        0      643 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_expansion.py
+-rw-r--r--   0        0        0     1921 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_field.py
+-rw-r--r--   0        0        0      288 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_geo.py
+-rw-r--r--   0        0        0      231 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_geo_coordinates.py
+-rw-r--r--   0        0        0      111 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_id.py
+-rw-r--r--   0        0        0      287 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_non_public_metrics.py
+-rw-r--r--   0        0        0      285 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_organic_metrics.py
+-rw-r--r--   0        0        0      286 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_promoted_metrics.py
+-rw-r--r--   0        0        0      437 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_public_metrics.py
+-rw-r--r--   0        0        0      267 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_referenced_tweet.py
+-rw-r--r--   0        0        0     7079 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_response_body.py
+-rw-r--r--   0        0        0      417 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_user/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_user/user.py
+-rw-r--r--   0        0        0      168 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_user/user_expantion.py
+-rw-r--r--   0        0        0      619 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_user/user_field.py
+-rw-r--r--   0        0        0       65 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_user/user_id.py
+-rw-r--r--   0        0        0      108 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_user/user_verified_type.py
+-rw-r--r--   0        0        0      139 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/types/v2_user/username.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/utils/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/utils/_datetime.py
+-rw-r--r--   0        0        0      716 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/utils/_functional.py
+-rw-r--r--   0        0        0      904 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/utils/_oauth.py
+-rw-r--r--   0        0        0      790 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/utils/json.py
+-rw-r--r--   0        0        0      630 2023-05-19 00:41:37.730858 twitter_api_py-0.7.2/twitter_api/warning.py
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 twitter_api_py-0.7.2/PKG-INFO
```

### Comparing `twitter_api_py-0.7.1/LICENSE` & `twitter_api_py-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/README.md` & `twitter_api_py-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/pyproject.toml` & `twitter_api_py-0.7.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 authors = ["yassun4dev <yassun4dev@outlook.com>"]
 description = "Twitter API Client by Typed Python."
 name = "twitter-api-py"
-packages = [{include = "twitter_api"}]
+packages = [{ include = "twitter_api" }]
 readme = "README.md"
-version = "0.7.1"
+version = "0.7.2"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/twitter-api-py"
 classifiers = [
-    "Development Status :: 4 - Beta",
-    "Topic :: Software Development :: Libraries",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: BSD License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3 :: Only",
+  "Development Status :: 4 - Beta",
+  "Topic :: Software Development :: Libraries",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: BSD License",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3 :: Only",
 ]
 
 [tool.taskipy.tasks]
 test = "pytest"
 format = "black --target-version py310 ."
 lint = "PYRIGHT_PYTHON_FORCE_VERSION=latest pyright twitter_api/** tests/** examples/**"
 
@@ -60,11 +60,8 @@
 exclude = ["**/__pycache__"]
 reportPrivateImportUsage = "none"
 reportUnusedImport = true
 
 [tool.mypy]
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
-module = [
-  "colorama",
-  "authlib",
-]
+module = ["colorama", "authlib"]
```

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/session_resources.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/session_resources.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/twitter_oauth1_real_session.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/twitter_oauth1_real_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/twitter_oauth1_session.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/twitter_oauth1_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/twitter_oauth2_real_session.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/twitter_oauth2_real_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/oauth_session/twitter_oauth2_session.py` & `twitter_api_py-0.7.2/twitter_api/client/oauth_session/twitter_oauth2_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/request/request_async_client.py` & `twitter_api_py-0.7.2/twitter_api/client/request/request_async_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/request/request_async_real_client.py` & `twitter_api_py-0.7.2/twitter_api/client/request/request_async_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/request/request_client.py` & `twitter_api_py-0.7.2/twitter_api/client/request/request_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/request/request_mock_client.py` & `twitter_api_py-0.7.2/twitter_api/client/request/request_mock_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Generic, Optional, Union
 
 from typing_extensions import Self, Type, override
 
 from twitter_api.error import (
     MockInjectionResponseWrong,
+    MockResponseBodyRemainsError,
     MockResponseNotFound,
     TwitterApiError,
 )
 from twitter_api.rate_limit.manager.no_operation_rate_limit_manager import (
     NoOperationRateLimitManager,
 )
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
@@ -21,15 +22,15 @@
     QuryParameters,
     RequestClient,
     RequestJsonBody,
     ResponseModelBody,
 )
 
 
-class RequestMockClient(RequestClient, Generic[ResponseModelBody]):
+class _RequestMockClient(RequestClient, Generic[ResponseModelBody]):
     def __init__(
         self,
         *,
         oauth_version: OAuthVersion,
         rate_limit_target: RateLimitTarget,
         rate_limit_manager: RateLimitManager,
     ):
@@ -115,15 +116,18 @@
         url: Optional[Url] = None,
         auth: bool = True,
         headers: Optional[Headers] = None,
         query: Optional[QuryParameters] = None,
     ) -> ResponseModelBody:
         return self._extract_response_body(endpoint)
 
+
+class RequestMockClient(_RequestMockClient):
     def close(self) -> None:
-        pass
+        if len(self._store) != 0:
+            raise MockResponseBodyRemainsError()
 
     def __enter__(self) -> Self:
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
-        pass
+        self.close()
```

### Comparing `twitter_api_py-0.7.1/twitter_api/client/request/request_real_client.py` & `twitter_api_py-0.7.2/twitter_api/client/request/request_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/client/twitter_api_async_client.py` & `twitter_api_py-0.7.2/twitter_api/client/twitter_api_async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,15 +396,15 @@
         event_hooks: Optional[Mapping[str, list[httpx.EventHook]]] = None,
         limits: httpx.Limits = httpx.DEFAULT_LIMITS,
         mounts: Optional[Mapping[str, httpx.AsyncBaseTransport]] = None,
         proxies: Optional[httpx.ProxiesTypes] = None,
         timeout: httpx.TimeoutTypes = httpx.DEFAULT_TIMEOUT_CONFIG,
         transport: Optional[httpx.AsyncBaseTransport] = None,
         verify: httpx.VerifyTypes = True,
-    ):
+    ) -> Self:
         """OAuth 2.0 の Bearer 認証を用いてクライアントを作成する。"""
 
         from twitter_api.client.twitter_api_async_real_client import (
             TwitterApiAsyncRealClient,
         )
 
         return TwitterApiAsyncRealClient.from_oauth2_bearer_token(
@@ -427,15 +427,15 @@
         event_hooks: Optional[Mapping[str, list[httpx.EventHook]]] = None,
         limits: httpx.Limits = httpx.DEFAULT_LIMITS,
         mounts: Optional[Mapping[str, httpx.AsyncBaseTransport]] = None,
         proxies: Optional[httpx.ProxiesTypes] = None,
         timeout: httpx.TimeoutTypes = httpx.DEFAULT_TIMEOUT_CONFIG,
         transport: Optional[httpx.AsyncBaseTransport] = None,
         verify: httpx.VerifyTypes = True,
-    ):
+    ) -> Self:
         """環境変数から、 OAuth 2.0 の Bearer 認証を用いてクライアントを作成する。"""
 
         return cls.from_oauth2_bearer_token(
             cls._get_env(bearer_token_env),
             rate_limit_manager=rate_limit_manager,
             event_hooks=event_hooks,
             limits=limits,
@@ -456,15 +456,15 @@
         event_hooks: Optional[Mapping[str, list[httpx.EventHook]]] = None,
         limits: httpx.Limits = httpx.DEFAULT_LIMITS,
         mounts: Optional[Mapping[str, httpx.AsyncBaseTransport]] = None,
         proxies: Optional[httpx.ProxiesTypes] = None,
         timeout: httpx.TimeoutTypes = httpx.DEFAULT_TIMEOUT_CONFIG,
         transport: Optional[httpx.AsyncBaseTransport] = None,
         verify: httpx.VerifyTypes = True,
-    ):
+    ) -> Self:
         """OAuth 2.0 のアプリ認証を用いてクライアントを作成する。"""
 
         from twitter_api.client.twitter_api_async_real_client import (
             TwitterApiAsyncRealClient,
         )
 
         return TwitterApiAsyncRealClient.from_oauth2_app(
@@ -490,15 +490,15 @@
         event_hooks: Optional[Mapping[str, list[httpx.EventHook]]] = None,
         limits: httpx.Limits = httpx.DEFAULT_LIMITS,
         mounts: Optional[Mapping[str, httpx.AsyncBaseTransport]] = None,
         proxies: Optional[httpx.ProxiesTypes] = None,
         timeout: httpx.TimeoutTypes = httpx.DEFAULT_TIMEOUT_CONFIG,
         transport: Optional[httpx.AsyncBaseTransport] = None,
         verify: httpx.VerifyTypes = True,
-    ):
+    ) -> Self:
         """環境変数から、OAuth 2.0 のアプリ認証を用いてクライアントを作成する。"""
 
         return cls.from_oauth2_app(
             api_key=cls._get_env(api_key_env),
             api_secret=cls._get_env(api_secret_env),
             rate_limit_manager=rate_limit_manager,
             event_hooks=event_hooks,
@@ -689,15 +689,15 @@
         event_hooks: Optional[Mapping[str, list[httpx.EventHook]]] = None,
         limits: httpx.Limits = httpx.DEFAULT_LIMITS,
         mounts: Optional[Mapping[str, httpx.AsyncBaseTransport]] = None,
         proxies: Optional[httpx.ProxiesTypes] = None,
         timeout: httpx.TimeoutTypes = httpx.DEFAULT_TIMEOUT_CONFIG,
         transport: Optional[httpx.AsyncBaseTransport] = None,
         verify: httpx.VerifyTypes = True,
-    ):
+    ) -> Self:
         """OAuth1.0a のアプリ認証を用いてクライアントを作成する。"""
 
         from twitter_api.client.twitter_api_async_real_client import (
             TwitterApiAsyncRealClient,
         )
 
         return TwitterApiAsyncRealClient.from_oauth1_app(
@@ -727,15 +727,15 @@
         event_hooks: Optional[Mapping[str, list[httpx.EventHook]]] = None,
         limits: httpx.Limits = httpx.DEFAULT_LIMITS,
         mounts: Optional[Mapping[str, httpx.AsyncBaseTransport]] = None,
         proxies: Optional[httpx.ProxiesTypes] = None,
         timeout: httpx.TimeoutTypes = httpx.DEFAULT_TIMEOUT_CONFIG,
         transport: Optional[httpx.AsyncBaseTransport] = None,
         verify: httpx.VerifyTypes = True,
-    ):
+    ) -> Self:
         """環境変数から、OAuth1.0a のアプリ認証を用いてクライアントを作成する。"""
 
         return cls.from_oauth1_app(
             api_key=cls._get_env(api_key_env),
             api_secret=cls._get_env(api_secret_env),
             access_token=cls._get_env(access_token_env),
             access_secret=cls._get_env(access_secret_env),
@@ -905,11 +905,19 @@
             verify=verify,
         )
 
     @abstractmethod
     async def aclose(self) -> None:
         ...
 
+    @abstractmethod
+    async def __aenter__(self) -> Self:
+        ...
+
+    @abstractmethod
+    async def __aexit__(self, exc_type, exc_value, traceback) -> None:
+        ...
+
     @classmethod
     def _get_env(cls, key: Env[str]) -> str:
         """環境変数を取り出す。"""
         return os.environ[key]
```

### Comparing `twitter_api_py-0.7.1/twitter_api/client/twitter_api_async_mock_client.py` & `twitter_api_py-0.7.2/twitter_api/client/twitter_api_async_mock_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,14 +386,17 @@
             timeout=timeout,
             transport=transport,
             verify=verify,
         )
 
     @override
     async def aclose(self) -> None:
-        pass
+        self._client.close()
 
+    @override
     async def __aenter__(self) -> Self:
+        self._client.__enter__()
         return self
 
+    @override
     async def __aexit__(self, exc_type, exc_value, traceback) -> None:
-        pass
+        self._client.__exit__(exc_type, exc_value, traceback)
```

### Comparing `twitter_api_py-0.7.1/twitter_api/client/twitter_api_async_real_client.py` & `twitter_api_py-0.7.2/twitter_api/client/twitter_api_async_real_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,13 +393,15 @@
             session=session,
         )
 
     @override
     async def aclose(self) -> None:
         await self._real_request_client.aclose()
 
+    @override
     async def __aenter__(self) -> Self:
         await self._real_request_client.__aenter__()
         return self
 
+    @override
     async def __aexit__(self, exc_type, exc_value, traceback) -> None:
         await self._real_request_client.__aexit__(exc_type, exc_value, traceback)
```

### Comparing `twitter_api_py-0.7.1/twitter_api/client/twitter_api_client.py` & `twitter_api_py-0.7.2/twitter_api/client/twitter_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
         event_hooks: Optional[Mapping[str, list[httpx.EventHook]]] = None,
         limits: httpx.Limits = httpx.DEFAULT_LIMITS,
         mounts: Optional[Mapping[str, httpx.BaseTransport]] = None,
         proxies: Optional[httpx.ProxiesTypes] = None,
         timeout: httpx.TimeoutTypes = httpx.DEFAULT_TIMEOUT_CONFIG,
         transport: Optional[httpx.BaseTransport] = None,
         verify: httpx.VerifyTypes = True,
-    ):
+    ) -> Self:
         """OAuth 2.0 の Bearer 認証を用いてクライアントを作成する。"""
 
         from .twitter_api_real_client import TwitterApiRealClient
 
         return TwitterApiRealClient.from_oauth2_bearer_token(
             bearer_token,
             rate_limit_manager=rate_limit_manager,
@@ -423,15 +423,15 @@
         event_hooks: Optional[Mapping[str, list[httpx.EventHook]]] = None,
         limits: httpx.Limits = httpx.DEFAULT_LIMITS,
         mounts: Optional[Mapping[str, httpx.BaseTransport]] = None,
         proxies: Optional[httpx.ProxiesTypes] = None,
         timeout: httpx.TimeoutTypes = httpx.DEFAULT_TIMEOUT_CONFIG,
         transport: Optional[httpx.BaseTransport] = None,
         verify: httpx.VerifyTypes = True,
-    ):
+    ) -> Self:
         """環境変数から、 OAuth 2.0 の Bearer 認証を用いてクライアントを作成する。"""
 
         return cls.from_oauth2_bearer_token(
             cls._get_env(bearer_token_env),
             rate_limit_manager=rate_limit_manager,
             event_hooks=event_hooks,
             limits=limits,
@@ -452,15 +452,15 @@
         event_hooks: Optional[Mapping[str, list[httpx.EventHook]]] = None,
         limits: httpx.Limits = httpx.DEFAULT_LIMITS,
         mounts: Optional[Mapping[str, httpx.BaseTransport]] = None,
         proxies: Optional[httpx.ProxiesTypes] = None,
         timeout: httpx.TimeoutTypes = httpx.DEFAULT_TIMEOUT_CONFIG,
         transport: Optional[httpx.BaseTransport] = None,
         verify: httpx.VerifyTypes = True,
-    ):
+    ) -> Self:
         """OAuth 2.0 のアプリ認証を用いてクライアントを作成する。"""
 
         from .twitter_api_real_client import TwitterApiRealClient
 
         return TwitterApiRealClient.from_oauth2_app(
             api_key=api_key,
             api_secret=api_secret,
@@ -484,15 +484,15 @@
         event_hooks: Optional[Mapping[str, list[httpx.EventHook]]] = None,
         limits: httpx.Limits = httpx.DEFAULT_LIMITS,
         mounts: Optional[Mapping[str, httpx.BaseTransport]] = None,
         proxies: Optional[httpx.ProxiesTypes] = None,
         timeout: httpx.TimeoutTypes = httpx.DEFAULT_TIMEOUT_CONFIG,
         transport: Optional[httpx.BaseTransport] = None,
         verify: httpx.VerifyTypes = True,
-    ):
+    ) -> Self:
         """環境変数から、OAuth 2.0 のアプリ認証を用いてクライアントを作成する。"""
 
         return cls.from_oauth2_app(
             api_key=cls._get_env(api_key_env),
             api_secret=cls._get_env(api_secret_env),
             rate_limit_manager=rate_limit_manager,
             event_hooks=event_hooks,
@@ -688,15 +688,15 @@
         event_hooks: Optional[Mapping[str, list[httpx.EventHook]]] = None,
         limits: httpx.Limits = httpx.DEFAULT_LIMITS,
         mounts: Optional[Mapping[str, httpx.BaseTransport]] = None,
         proxies: Optional[httpx.ProxiesTypes] = None,
         timeout: httpx.TimeoutTypes = httpx.DEFAULT_TIMEOUT_CONFIG,
         transport: Optional[httpx.BaseTransport] = None,
         verify: httpx.VerifyTypes = True,
-    ):
+    ) -> Self:
         """OAuth1.0a のアプリ認証を用いてクライアントを作成する。"""
 
         from .twitter_api_real_client import TwitterApiRealClient
 
         return TwitterApiRealClient.from_oauth1_app(
             api_key=api_key,
             api_secret=api_secret,
@@ -724,15 +724,15 @@
         event_hooks: Optional[Mapping[str, list[httpx.EventHook]]] = None,
         limits: httpx.Limits = httpx.DEFAULT_LIMITS,
         mounts: Optional[Mapping[str, httpx.BaseTransport]] = None,
         proxies: Optional[httpx.ProxiesTypes] = None,
         timeout: httpx.TimeoutTypes = httpx.DEFAULT_TIMEOUT_CONFIG,
         transport: Optional[httpx.BaseTransport] = None,
         verify: httpx.VerifyTypes = True,
-    ):
+    ) -> Self:
         """環境変数から、OAuth1.0a のアプリ認証を用いてクライアントを作成する。"""
 
         return cls.from_oauth1_app(
             api_key=cls._get_env(api_key_env),
             api_secret=cls._get_env(api_secret_env),
             access_token=cls._get_env(access_token_env),
             access_secret=cls._get_env(access_secret_env),
@@ -906,11 +906,19 @@
             verify=verify,
         )
 
     @abstractmethod
     def close(self) -> None:
         ...
 
+    @abstractmethod
+    def __enter__(self) -> Self:
+        ...
+
+    @abstractmethod
+    def __exit__(self, exc_type, exc_value, traceback) -> None:
+        ...
+
     @classmethod
     def _get_env(cls, key: Env[str]) -> str:
         """環境変数を取り出す。"""
         return os.environ[key]
```

### Comparing `twitter_api_py-0.7.1/twitter_api/client/twitter_api_mock_client.py` & `twitter_api_py-0.7.2/twitter_api/client/twitter_api_mock_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Mapping, Optional, Union
 
 from typing_extensions import Self, overload, override
 
+from twitter_api.client.twitter_api_client import TwitterApiClient
 from twitter_api.error import TwitterApiError
 from twitter_api.rate_limit.manager import DEFAULT_RATE_LIMIT_MANAGER
 from twitter_api.rate_limit.manager.rate_limit_manager import RateLimitManager
 from twitter_api.rate_limit.rate_limit_target import RateLimitTarget
 from twitter_api.resources.oauth2_invalidate_token import Oauth2InvalidateTokenUrl
 from twitter_api.resources.oauth2_invalidate_token.post_oauth2_invalidate_token import (
     PostOauth2InvalidateTokenResponseBody,
@@ -110,15 +111,14 @@
     Env,
     OAuthVersion,
 )
 from twitter_api.types.v2_scope import Scope
 
 from .request.request_client import RequestClient
 from .request.request_mock_client import RequestMockClient
-from .twitter_api_client import TwitterApiClient
 
 
 class _BaseTwitterApiMockClient:
     def __init__(
         self,
         *,
         oauth_version: OAuthVersion,
@@ -805,14 +805,18 @@
             timeout=timeout,
             transport=transport,
             verify=verify,
         )
 
     @override
     def close(self) -> None:
-        pass
+        self._client.close()
 
+    @override
     def __enter__(self) -> Self:
+        self._client.__enter__()
+
         return self
 
+    @override
     def __exit__(self, exc_type, exc_value, traceback) -> None:
-        pass
+        self._client.__exit__(exc_type, exc_value, traceback)
```

### Comparing `twitter_api_py-0.7.1/twitter_api/client/twitter_api_real_client.py` & `twitter_api_py-0.7.2/twitter_api/client/twitter_api_real_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,14 +374,16 @@
             session=session,
         )
 
     @override
     def close(self) -> None:
         self._real_request_client.close()
 
+    @override
     def __enter__(self) -> Self:
         self._real_request_client.__enter__()
 
         return self
 
+    @override
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         self._real_request_client.__exit__(exc_type, exc_value, traceback)
```

### Comparing `twitter_api_py-0.7.1/twitter_api/error.py` & `twitter_api_py-0.7.2/twitter_api/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,20 @@
             **dict(
                 expected_endpoint=self.expected_endpoint,
                 endpoint=self.endpoint,
             ),
         )
 
 
+class MockResponseBodyRemainsError(TwitterApiError):
+    @property
+    def message(self) -> str:
+        return "モックとして出力したいデータが残っています。"
+
+
 class TwitterApiResponseModelBodyDecodeError(TwitterApiError):
     def __init__(self, endpoint: Endpoint, content: bytes, **extra):
         self.endpoint = endpoint
         self.content = content
         self._extra = extra
 
     @property
```

### Comparing `twitter_api_py-0.7.1/twitter_api/rate_limit/manager/__init__.py` & `twitter_api_py-0.7.2/twitter_api/rate_limit/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/rate_limit/manager/dict_rate_limit_manager.py` & `twitter_api_py-0.7.2/twitter_api/rate_limit/manager/dict_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py` & `twitter_api_py-0.7.2/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/rate_limit/manager/mixins/dict_rate_limit_checker_mixin.py` & `twitter_api_py-0.7.2/twitter_api/rate_limit/manager/mixins/dict_rate_limit_checker_mixin.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/rate_limit/manager/mixins/raise_rate_limit_handler_mixin.py` & `twitter_api_py-0.7.2/twitter_api/rate_limit/manager/mixins/raise_rate_limit_handler_mixin.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/rate_limit/manager/mixins/sleep_rate_limit_handler_mixin.py` & `twitter_api_py-0.7.2/twitter_api/rate_limit/manager/mixins/sleep_rate_limit_handler_mixin.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py` & `twitter_api_py-0.7.2/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/rate_limit/manager/rate_limit_manager.py` & `twitter_api_py-0.7.2/twitter_api/rate_limit/manager/rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/rate_limit/rate_limit.py` & `twitter_api_py-0.7.2/twitter_api/rate_limit/rate_limit.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py` & `twitter_api_py-0.7.2/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/oauth2_token/post_oauth2_token.py` & `twitter_api_py-0.7.2/twitter_api/resources/oauth2_token/post_oauth2_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversation_messages/__init__.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversation_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_tweet/delete_v2_tweet.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_tweet/delete_v2_tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_tweet/get_v2_tweet.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_tweet/get_v2_tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_tweets/get_v2_tweets.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_tweets/get_v2_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_tweets/post_v2_tweets.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_tweets/post_v2_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_user/get_v2_user.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_user/get_v2_user.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_user_followers/get_v2_user_followers.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_user_followers/get_v2_user_followers.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_user_following/post_v2_user_following.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_user_following/post_v2_user_following.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_users/get_v2_users.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_users/get_v2_users.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_users_by/get_v2_users_by.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_users_by/get_v2_users_by.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py` & `twitter_api_py-0.7.2/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/_generic_client.py` & `twitter_api_py-0.7.2/twitter_api/types/_generic_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/_model.py` & `twitter_api_py-0.7.2/twitter_api/types/_model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/_paging.py` & `twitter_api_py-0.7.2/twitter_api/types/_paging.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/comma_separatable.py` & `twitter_api_py-0.7.2/twitter_api/types/comma_separatable.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/extra_permissive_model.py` & `twitter_api_py-0.7.2/twitter_api/types/extra_permissive_model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/http.py` & `twitter_api_py-0.7.2/twitter_api/types/http.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/httpx.py` & `twitter_api_py-0.7.2/twitter_api/types/httpx.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/oauth.py` & `twitter_api_py-0.7.2/twitter_api/types/oauth.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/oauth1/oauth1_access_token.py` & `twitter_api_py-0.7.2/twitter_api/types/oauth1/oauth1_access_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/oauth1/oauth1_authorization.py` & `twitter_api_py-0.7.2/twitter_api/types/oauth1/oauth1_authorization.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/oauth2/oauth2_access_token.py` & `twitter_api_py-0.7.2/twitter_api/types/oauth2/oauth2_access_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/oauth2/oauth2_authorization.py` & `twitter_api_py-0.7.2/twitter_api/types/oauth2/oauth2_authorization.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_dm_conversation/dm_conversation_message.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_dm_conversation/dm_conversation_message.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_language.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_language.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_media/media.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_media/media.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_media/media_field.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_media/media_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_place/place.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_place/place.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_place/place_country_code.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_place/place_country_code.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_poll/poll.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_poll/poll.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_retweet/retweet_entities_description.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_retweet/retweet_entities_description.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_scope.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_scope.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/_and_operator.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/_and_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/_not_operator.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/_not_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/_or_operator.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/_or_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/bounding_box_operator.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/bounding_box_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/context_operator.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/context_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/group_operator.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/group_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/operator.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class CompleteOperator(Operator):
     """
     検索クエリとして成り立っている Operator。
     """
 
-    def __and__(self, other: Operator):
+    def __and__(self, other: Operator) -> "CompleteOperator":
         from ._and_operator import CompleteAndOperator
 
         return CompleteAndOperator(self, other)
 
     @overload
     def __or__(self, other: "CompleteOperator") -> "CompleteOperator":
         ...
```

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/place_operator.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/place_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_search_query/operators/point_radius_operator.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_search_query/operators/point_radius_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_search_query/search_query.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_search_query/search_query.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_search_query/search_query_builder.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_search_query/search_query_builder.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_entities.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_entities.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_expansion.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_expansion.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_field.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_tweet/tweet_response_body.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_tweet/tweet_response_body.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_user/user.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_user/user.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/types/v2_user/user_field.py` & `twitter_api_py-0.7.2/twitter_api/types/v2_user/user_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/utils/_functional.py` & `twitter_api_py-0.7.2/twitter_api/utils/_functional.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/utils/_oauth.py` & `twitter_api_py-0.7.2/twitter_api/utils/_oauth.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/utils/json.py` & `twitter_api_py-0.7.2/twitter_api/utils/json.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/twitter_api/warning.py` & `twitter_api_py-0.7.2/twitter_api/warning.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.7.1/PKG-INFO` & `twitter_api_py-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-py
-Version: 0.7.1
+Version: 0.7.2
 Summary: Twitter API Client by Typed Python.
 Home-page: https://github.com/yassun4dev/twitter-api-py
 License: BSD-3-Clause
 Author: yassun4dev
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

