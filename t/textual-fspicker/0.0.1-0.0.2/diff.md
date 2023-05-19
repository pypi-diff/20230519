# Comparing `tmp/textual_fspicker-0.0.1-py3-none-any.whl.zip` & `tmp/textual_fspicker-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 9656 bytes, number of entries: 10
--rw-r--r--  2.0 unx      692 b- defN 23-May-17 19:56 textual_fspicker/__init__.py
+Zip file size: 10971 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      692 b- defN 23-May-19 09:53 textual_fspicker/__init__.py
 -rw-r--r--  2.0 unx     1159 b- defN 23-May-18 19:46 textual_fspicker/__main__.py
--rw-r--r--  2.0 unx     4625 b- defN 23-May-18 19:53 textual_fspicker/file_open.py
+-rw-r--r--  2.0 unx     6739 b- defN 23-May-19 09:53 textual_fspicker/file_open.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-18 20:02 textual_fspicker/py.typed
+-rw-r--r--  2.0 unx     2174 b- defN 23-May-19 09:53 textual_fspicker/safe_tests.py
 -rw-r--r--  2.0 unx      389 b- defN 23-May-17 19:18 textual_fspicker/parts/__init__.py
--rw-r--r--  2.0 unx    12704 b- defN 23-May-17 19:56 textual_fspicker/parts/directory_navigation.py
--rw-r--r--  2.0 unx     5249 b- defN 23-May-18 20:26 textual_fspicker-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 20:26 textual_fspicker-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-18 20:26 textual_fspicker-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      862 b- defN 23-May-18 20:26 textual_fspicker-0.0.1.dist-info/RECORD
-10 files, 25789 bytes uncompressed, 8166 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx    11908 b- defN 23-May-19 09:53 textual_fspicker/parts/directory_navigation.py
+-rw-r--r--  2.0 unx     5250 b- defN 23-May-19 09:53 textual_fspicker-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-19 09:53 textual_fspicker-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-19 09:53 textual_fspicker-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      949 b- defN 23-May-19 09:53 textual_fspicker-0.0.2.dist-info/RECORD
+11 files, 29369 bytes uncompressed, 9345 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -6,26 +6,29 @@
 
 Filename: textual_fspicker/file_open.py
 Comment: 
 
 Filename: textual_fspicker/py.typed
 Comment: 
 
+Filename: textual_fspicker/safe_tests.py
+Comment: 
+
 Filename: textual_fspicker/parts/__init__.py
 Comment: 
 
 Filename: textual_fspicker/parts/directory_navigation.py
 Comment: 
 
-Filename: textual_fspicker-0.0.1.dist-info/METADATA
+Filename: textual_fspicker-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: textual_fspicker-0.0.1.dist-info/WHEEL
+Filename: textual_fspicker-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: textual_fspicker-0.0.1.dist-info/top_level.txt
+Filename: textual_fspicker-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: textual_fspicker-0.0.1.dist-info/RECORD
+Filename: textual_fspicker-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## textual_fspicker/__init__.py

```diff
@@ -3,15 +3,15 @@
 ######################################################################
 # Main app information.
 __author__     = "Dave Pearson"
 __copyright__  = "Copyright 2023, Dave Pearson"
 __credits__    = [ "Dave Pearson" ]
 __maintainer__ = "Dave Pearson"
 __email__      = "davep@davep.org"
-__version__    = "0.0.1"
+__version__    = "0.0.2"
 __licence__    = "MIT"
 
 ##############################################################################
 # Local imports.
 from .file_open import FileOpen
 
 ##############################################################################
```

## textual_fspicker/file_open.py

```diff
@@ -15,53 +15,61 @@
 from textual.widgets    import Button, Input
 
 ##############################################################################
 # Local imports.
 from .parts import DirectoryNavigation
 
 ##############################################################################
+class Dialog( Vertical ):
+    """Layout class for the main dialog area."""
+
+##############################################################################
+class InputBar( Horizontal ):
+    """The input bar area of the dialog."""
+
+##############################################################################
 class FileOpen( ModalScreen[ Path ] ):
     """A file opening dialog."""
 
     DEFAULT_CSS = """
     FileOpen {
         align: center middle;
     }
 
-    FileOpen > Vertical#dialog {
+    FileOpen Dialog {
         width: 80%;
         height: 80%;
         border: panel $panel-lighten-2;
         background: $panel-lighten-1;
         border-title-color: $text;
         border-title-background: $panel-lighten-2;
         border-subtitle-color: $text;
         border-subtitle-background: $error;
     }
 
-    FileOpen Horizontal#input {
+    FileOpen InputBar {
         height: auto;
         align: right middle;
         padding-top: 1;
         padding-right: 1;
         padding-bottom: 1;
     }
 
-    FileOpen Horizontal#input Button {
+    FileOpen InputBar Button {
         margin-left: 1;
     }
 
-    FileOpen Horizontal#input Input {
+    FileOpen InputBar Input {
         width: 1fr;
     }
     """
 
     BINDINGS = [
         Binding( "escape", "dismiss" ),
-        Binding( "full_stop", "hidden")
+        Binding( "full_stop", "hidden" )
     ]
     """The bindings for the dialog."""
 
     def __init__( self, location: str | Path | None=None, title: str="Open", must_exist: bool=True ) -> None:
         """Initialise the `FileOpen` dialog.
 
         Args:
@@ -79,71 +87,115 @@
 
     def compose( self ) -> ComposeResult:
         """Compose the child widgets.
 
         Returns:
             The widgets to compose.
         """
-        with Vertical( id="dialog" ) as dialog:
+        with Dialog() as dialog:
             dialog.border_title = self._title
             yield DirectoryNavigation(self._location)
-            with Horizontal( id="input" ):
+            with InputBar():
                 yield Input()
                 yield Button( "Open", id="open" )
                 yield Button( "Cancel", id="cancel" )
 
     def _set_error( self, message: str="" ) -> None:
         """Set or clear the error message.
 
         Args:
             message: Optional message to show as an error.
         """
-        self.query_one( "#dialog", Vertical ).border_subtitle = message
+        self.query_one( Dialog ).border_subtitle = message
 
     @on( DirectoryNavigation.Selected )
     def _select_file( self, event: DirectoryNavigation.Selected ) -> None:
         """Handle a file being selected in the picker.
 
         Args:
             event: The event to handle.
         """
         file_name       = self.query_one( Input )
         file_name.value = str( event.path.name )
         file_name.focus()
 
+    @on( DirectoryNavigation.PermissionError )
+    def _show_permission_error( self ) -> None:
+        """Show any permission error bubbled up from the directory navigator."""
+        self._set_error( "Permission error" )
+
     @on( Input.Submitted )
     @on( Button.Pressed, "#open" )
     def _confirm_file( self, event: Input.Submitted | Button.Pressed ) -> None:
         """Confirm the selection of the file in the input box.
 
         Args:
             event: The event to handle.
         """
         event.stop()
         file_name = self.query_one( Input )
+
+        # Only even try and process this if there's some input.
         if file_name.value:
-            chosen = self.query_one( DirectoryNavigation ).location / file_name.value
+
+            # If it looks like the user is typing in some sort of home
+            # directory path... (does pathlib let me test for this, or at
+            # least ask what the home character is? Docs don't mention this;
+            # so for now I'm going to hard-code this).
+            if file_name.value.startswith( "~" ):
+                # ...let's simply expand and go with that.
+                try:
+                    chosen = Path( file_name.value ).expanduser()
+                except RuntimeError as error:
+                    self._set_error( str( error ) )
+                    return
+            else:
+                # It's not a home directory path, so let's combine with the
+                # location of the directory navigator widget.
+                chosen = (
+                    self.query_one( DirectoryNavigation ).location / file_name.value
+                ).resolve()
+
+            # If it's a directory, approach it like it's the user simply
+            # doing a "cd".
+            try:
+                if chosen.is_dir():
+                    self.query_one( Input ).value                  = ""
+                    self.query_one( DirectoryNavigation ).location = chosen
+                    self.query_one( DirectoryNavigation ).focus()
+                    return
+            except PermissionError:
+                self._set_error( "Permission error" )
+                return
+
+            # At this point it's something that can be picked. Do the "must
+            # exist" test if needed.
             if self._must_exist and not chosen.exists():
                 self._set_error( "The file must exist" )
                 return
+
+            # Finally, we've got some sort of pickable item and it's good to
+            # be picked. Let's go with it.
             self.dismiss( result=chosen )
+
         else:
             self._set_error( "A file must be chosen" )
 
     @on( Button.Pressed, "#cancel" )
     def _cancel( self, event: Button.Pressed ) -> None:
         """Cancel the dialog.
 
         Args:
             event: The even to handle.
         """
         event.stop()
         self.dismiss()
 
     @on( Input.Changed )
+    @on( DirectoryNavigation.Changed )
     def _clear_error( self ) -> None:
         """Clear any error that might be showing."""
         self._set_error()
 
     def action_hidden( self ) -> None:
         """Action for toggling the display of hidden files."""
         self.query_one( DirectoryNavigation ).toggle_hidden()
```

## textual_fspicker/parts/directory_navigation.py

```diff
@@ -21,14 +21,18 @@
 from textual.reactive            import var
 from textual.message             import Message
 from textual.widgets             import OptionList
 from textual.widgets.option_list import Option
 from textual.worker              import get_current_worker
 
 ##############################################################################
+# Local imports.
+from ..safe_tests import is_dir, is_file, is_symlink
+
+##############################################################################
 class DirectoryEntry( Option ):
     """A directory entry for the `DirectoryNaviation` class."""
 
     FOLDER_ICON: Final[ Text ] = Text.from_markup( ":file_folder:" )
     """The icon to use for a folder."""
 
     FILE_ICON: Final[ Text ] = Text.from_markup( ":page_facing_up:" )
@@ -48,15 +52,15 @@
         Args:
             location: The location to get the name for.
 
         Returns:
             The formatted name.
         """
         return Text.assemble(
-            location.name, " ", self.LINK_ICON if location.is_symlink() else ""
+            location.name, " ", self.LINK_ICON if is_symlink( location ) else ""
         )
 
     @staticmethod
     def _mtime( location: Path ) -> str:
         """Get a formatted modification time for the given location.
 
         Args:
@@ -84,77 +88,40 @@
         try:
             entry_size = location.stat().st_size
         except FileNotFoundError:
             entry_size = 0
         # TODO: format well for a file browser.
         return str( entry_size )
 
-    def _dir( self, prompt: Table, location: Path ) -> Table:
-        """Generate a prompt for a directory.
-
-        Args:
-            prompt: The table to populate.
-            location: The location to generate the prompt for.
-
-        Returns:
-            The populated table.
-        """
-        prompt.add_column( no_wrap=True, width=1 )
-        prompt.add_column( no_wrap=True, justify="left", width=3 )
-        prompt.add_column( no_wrap=True, justify="left", ratio=1 )
-        prompt.add_column( no_wrap=True, justify="right", width=10 )
-        prompt.add_column( no_wrap=True, justify="right", width=20 )
-        prompt.add_column( no_wrap=True, width=1 )
-        prompt.add_row(
-            "",
-            self.FOLDER_ICON,
-            self._name( location ),
-            self._size( location ),
-            self._mtime( location ),
-            ""
-        )
-        return prompt
-
-    def _file( self, prompt: Table, location: Path ) -> Table:
-        """Generate a prompt for a file.
+    def _as_renderable( self, location: Path ) -> RenderableType:
+        """Create the renderable for this entry.
 
         Args:
-            prompt: The table to populate.
-            location: The location to generate the prompt for.
+            location: The location to turn into a renderable.
 
         Returns:
-            The populated table
+            The entry as a Rich renderable.
         """
+        prompt = Table.grid( expand=True )
         prompt.add_column( no_wrap=True, width=1 )
         prompt.add_column( no_wrap=True, justify="left", width=3 )
         prompt.add_column( no_wrap=True, justify="left", ratio=1 )
         prompt.add_column( no_wrap=True, justify="right", width=10 )
         prompt.add_column( no_wrap=True, justify="right", width=20 )
         prompt.add_column( no_wrap=True, width=1 )
         prompt.add_row(
             "",
-            self.FILE_ICON,
+            self.FOLDER_ICON if is_dir( location ) else self.FILE_ICON,
             self._name( location ),
             self._size( location ),
             self._mtime( location ),
             ""
         )
         return prompt
 
-    def _as_renderable( self, location: Path ) -> RenderableType:
-        """Create the renderable for this entry.
-
-        Args:
-            location: The location to turn into a renderable.
-
-        Returns:
-            The entry as a Rich renderable.
-        """
-        return ( { True: self._dir, False: self._file }[ location.is_dir() ] )( Table.grid( expand=True ), location )
-
 ##############################################################################
 class DirectoryNavigation( OptionList ):
     """A directory navigation widget.
 
     Provides a single-pane widget that lets the user navigate their way
     through a filesystenm, changing in and out of directories, and selecting
     a file.
@@ -179,14 +146,17 @@
 
     class Highlighted( _PathMessage ):
         """Message sent when an entry in the display is highlighted."""
 
     class Selected( _PathMessage ):
         """Message sent when an entry in the filesystem is selected."""
 
+    class PermissionError( _PathMessage ):
+        """Message sent when there's a permission problem with a path."""
+
     _location: var[ Path ] = var[ Path ]( Path( "." ).absolute(), init=False )
     """The current location for the directory."""
 
     show_files: var[ bool ] = var( True )
     """Should files be shown and be selectable?"""
 
     show_hidden: var[ bool ] = var( False )
@@ -262,15 +232,15 @@
             `True` if the path should be hidden, `False` if not.
         """
         return self.is_hidden( path ) and not self.show_hidden
 
     def _sort( self, entries: Iterable[ DirectoryEntry ] ) -> Iterable[ DirectoryEntry ]:
         """Sort the entries as per the value of `sort_display`."""
         if self.sort_display:
-            return sorted( entries, key=lambda entry: ( not entry.location.is_dir(), entry.location.name ) )
+            return sorted( entries, key=lambda entry: ( not is_dir( entry.location ), entry.location.name ) )
         return entries
 
     def _repopulate_display( self ) -> None:
         """Repopulate the display of directories."""
         with self.app.batch_update():
             self.clear_options()
             if not self.is_root:
@@ -289,19 +259,22 @@
         # parallel copy of *all* possible options for the list and then
         # populate from that.
         self._entries = []
 
         # Now loop over the directory, looking for directories within and
         # streaming them into the list via the app thread.
         worker = get_current_worker()
-        for entry in self._location.iterdir():
-            if entry.is_dir() or ( entry.is_file() and self.show_files ):
-                self._entries.append( DirectoryEntry( self._location / entry.name ) )
-            if worker.is_cancelled:
-                return
+        try:
+            for entry in self._location.iterdir():
+                if is_dir( entry ) or ( is_file( entry ) and self.show_files ):
+                    self._entries.append( DirectoryEntry( self._location / entry.name ) )
+                if worker.is_cancelled:
+                    return
+        except PermissionError:
+            self.post_message( self.PermissionError( self, self._location ) )
 
         # Now that we've loaded everything up, let's make the call to update
         # the display.
         self.app.call_from_thread( self._repopulate_display )
 
     def _watch__location( self ) -> None:
         """Reload the content if the location changes."""
@@ -340,15 +313,15 @@
 
         Args:
             event: The event to handle.
         """
         event.stop()
         assert isinstance( event.option, DirectoryEntry )
         # If the use has selected a directory...
-        if event.option.location.is_dir():
+        if is_dir( event.option.location ):
             # ...we do navigation and don't post anything from here.
             self._location = event.option.location.resolve()
         else:
             # If it's not a directory it should be a file; that should be a
             # selection event.
             self.post_message( self.Selected( self, event.option.location ) )
```

## Comparing `textual_fspicker-0.0.1.dist-info/METADATA` & `textual_fspicker-0.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-fspicker
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Textual filesystem picker dialog library.
 Home-page: https://github.com/davep/textual-fspicker
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
@@ -29,15 +29,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: textual (>=0.25.0)
 
 # textual-fspicker
 
 ![Viewing its own directory](https://raw.githubusercontent.com/davep/textual-fspicker/main/img/textual-fspicker.png)
-*An example of `textual-fsicker` being used in a Textual application*
+*An example of `textual-fspicker` being used in a Textual application*
 
 ## Introduction
 
 This library provides a simple set of filesystem navigation and picking
 dialogs (actually, as of the time of writing, it only provides the one, this
 is a very early WiP you're seeing). The aim is to provide "ready to go"
 dialogs that should also be fairly easy to tailor to your own applications.
```

