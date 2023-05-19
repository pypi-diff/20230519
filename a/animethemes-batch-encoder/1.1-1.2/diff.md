# Comparing `tmp/animethemes-batch-encoder-1.1.tar.gz` & `tmp/animethemes-batch-encoder-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animethemes-batch-encoder-1.1.tar", last modified: Tue Apr 25 03:56:26 2023, max compression
+gzip compressed data, was "animethemes-batch-encoder-1.2.tar", last modified: Fri May 19 05:04:25 2023, max compression
```

## Comparing `animethemes-batch-encoder-1.1.tar` & `animethemes-batch-encoder-1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 03:56:26.935955 animethemes-batch-encoder-1.1/
--rw-rw-rw-   0        0        0     1088 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/LICENSE
--rw-rw-rw-   0        0        0     4216 2023-04-25 03:56:26.934953 animethemes-batch-encoder-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3313 2023-04-25 03:41:09.000000 animethemes-batch-encoder-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 03:56:26.927863 animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/
--rw-rw-rw-   0        0        0     4216 2023-04-25 03:56:26.000000 animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      590 2023-04-25 03:56:26.000000 animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 03:56:26.000000 animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 03:56:26.000000 animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-25 03:56:26.000000 animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 03:56:26.933954 animethemes-batch-encoder-1.1/batch_encoder/
--rw-rw-rw-   0        0        0        0 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/__init__.py
--rw-rw-rw-   0        0        0     6340 2023-04-25 03:41:09.000000 animethemes-batch-encoder-1.1/batch_encoder/__main__.py
--rw-rw-rw-   0        0        0     1280 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_bitrate_mode.py
--rw-rw-rw-   0        0        0     2615 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_colorspace.py
--rw-rw-rw-   0        0        0    12926 2023-04-25 03:41:09.000000 animethemes-batch-encoder-1.1/batch_encoder/_encode_webm.py
--rw-rw-rw-   0        0        0     3434 2023-04-25 03:41:09.000000 animethemes-batch-encoder-1.1/batch_encoder/_encoding_config.py
--rw-rw-rw-   0        0        0     2527 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_loudnorm_filter.py
--rw-rw-rw-   0        0        0      711 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_seek.py
--rw-rw-rw-   0        0        0     5615 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_seek_collector.py
--rw-rw-rw-   0        0        0     6593 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_source_file.py
--rw-rw-rw-   0        0        0     1375 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.1/batch_encoder/_utils.py
--rw-rw-rw-   0        0        0       42 2023-04-25 03:56:26.935955 animethemes-batch-encoder-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1194 2023-04-25 03:41:09.000000 animethemes-batch-encoder-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 05:04:25.590101 animethemes-batch-encoder-1.2/
+-rw-rw-rw-   0        0        0     1088 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/LICENSE
+-rw-rw-rw-   0        0        0     4321 2023-05-19 05:04:25.589100 animethemes-batch-encoder-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3418 2023-05-19 05:02:46.000000 animethemes-batch-encoder-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 05:04:25.581579 animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/
+-rw-rw-rw-   0        0        0     4321 2023-05-19 05:04:25.000000 animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2023-05-19 05:04:25.000000 animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 05:04:25.000000 animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 05:04:25.000000 animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-19 05:04:25.000000 animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 05:04:25.589100 animethemes-batch-encoder-1.2/batch_encoder/
+-rw-rw-rw-   0        0        0        0 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/__init__.py
+-rw-rw-rw-   0        0        0     6993 2023-05-19 05:02:46.000000 animethemes-batch-encoder-1.2/batch_encoder/__main__.py
+-rw-rw-rw-   0        0        0     1280 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/_bitrate_mode.py
+-rw-rw-rw-   0        0        0     2615 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/_colorspace.py
+-rw-rw-rw-   0        0        0    12970 2023-05-19 05:02:46.000000 animethemes-batch-encoder-1.2/batch_encoder/_encode_webm.py
+-rw-rw-rw-   0        0        0     3814 2023-05-19 05:02:46.000000 animethemes-batch-encoder-1.2/batch_encoder/_encoding_config.py
+-rw-rw-rw-   0        0        0     2527 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/_loudnorm_filter.py
+-rw-rw-rw-   0        0        0      711 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/_seek.py
+-rw-rw-rw-   0        0        0     5615 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/_seek_collector.py
+-rw-rw-rw-   0        0        0     6594 2023-05-19 05:02:46.000000 animethemes-batch-encoder-1.2/batch_encoder/_source_file.py
+-rw-rw-rw-   0        0        0     1375 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/_utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-19 05:04:25.590101 animethemes-batch-encoder-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1194 2023-05-19 05:02:46.000000 animethemes-batch-encoder-1.2/setup.py
```

### Comparing `animethemes-batch-encoder-1.1/LICENSE` & `animethemes-batch-encoder-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.1/PKG-INFO` & `animethemes-batch-encoder-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-batch-encoder
-Version: 1.1
+Version: 1.2
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -85,14 +85,16 @@
 
 `CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
 
 `Threads` is the number of threads used to encode. Default is 4.
 
 `LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
 
+`AlternateSourceEnable` is a flag for alternate command lines between source files. Default is False.
+
 `IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
 
 `VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
 
 **Logging**
 
 Determines the level of the logging for the program.
```

### Comparing `animethemes-batch-encoder-1.1/README.md` & `animethemes-batch-encoder-1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,16 @@
 
 `CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
 
 `Threads` is the number of threads used to encode. Default is 4.
 
 `LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
 
+`AlternateSourceEnable` is a flag for alternate command lines between source files. Default is False.
+
 `IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
 
 `VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
 
 **Logging**
 
 Determines the level of the logging for the program.
```

### Comparing `animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/PKG-INFO` & `animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-batch-encoder
-Version: 1.1
+Version: 1.2
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -85,14 +85,16 @@
 
 `CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
 
 `Threads` is the number of threads used to encode. Default is 4.
 
 `LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
 
+`AlternateSourceEnable` is a flag for alternate command lines between source files. Default is False.
+
 `IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
 
 `VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
 
 **Logging**
 
 Determines the level of the logging for the program.
```

### Comparing `animethemes-batch-encoder-1.1/animethemes_batch_encoder.egg-info/SOURCES.txt` & `animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.1/batch_encoder/__main__.py` & `animethemes-batch-encoder-1.2/batch_encoder/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     config_file = os.path.join(dirs.user_config_dir, args.configfile)
     if not os.path.exists(config_file):
         config['Encoding'] = {EncodingConfig.config_allowed_filetypes: EncodingConfig.default_allowed_filetypes,
                               EncodingConfig.config_encoding_modes: EncodingConfig.default_encoding_modes,
                               EncodingConfig.config_crfs: EncodingConfig.default_crfs,
                               EncodingConfig.config_threads: EncodingConfig.default_threads,
                               EncodingConfig.config_limit_size_enable: EncodingConfig.default_limit_size_enable,
+                              EncodingConfig.config_alternate_source_files: EncodingConfig.default_alternate_source_files,
                               EncodingConfig.config_include_unfiltered: EncodingConfig.default_include_unfiltered,
                               EncodingConfig.config_default_video_stream: '',
                               EncodingConfig.config_default_audio_stream: ''}
         config['VideoFilters'] = EncodingConfig.default_video_filters
 
         os.makedirs(os.path.dirname(config_file), exist_ok=True)
         with open(config_file, 'w', encoding='utf8') as f:
@@ -92,17 +93,29 @@
                     while not is_collector_valid:
                         seek_collector = SeekCollector(source_file)
                         is_collector_valid = seek_collector.is_valid()
 
                     for seek in seek_collector.get_seek_list():
                         logging.info(f'Generating commands with seek ss: \'{seek.ss}\', to: \'{seek.to}\'')
                         encode_webm = EncodeWebM(source_file, seek)
-                        commands = commands + encode_webm.get_commands(encoding_config)
+                        load_commands = encode_webm.get_commands(encoding_config)
+                        commands = commands + load_commands
                 except KeyboardInterrupt:
                     logging.info(f'Exiting from inclusion of file \'{source_file_candidate}\' after keyboard interrupt')
+        
+        # Alternate lines per source files
+        if encoding_config.alternate_source_files == True:
+            output_list = []
+            lines_per_source = len(load_commands)
+            for i in range(lines_per_source):
+                output_list.append(commands[i])
+                for k in range(1, len(commands) // lines_per_source):
+                    output_list.append(commands[i + lines_per_source * k])
+
+            commands = output_list
 
     # Write commands to file
     if args.mode == 1:
         logging.info(f'Writing {len(commands)} commands to file \'{args.file}\'...')
         with open(args.file, mode='w', encoding='utf8') as f:
             for command in commands:
                 f.write(command + '\n')
@@ -129,8 +142,8 @@
             subprocess.call(command, shell=True)
 
 
 if __name__ == '__main__':
     try:
         main()
     except KeyboardInterrupt:
-        logging.error('Exiting after keyboard interrupt')
+        logging.error('Exiting after keyboard interrupt')
```

### Comparing `animethemes-batch-encoder-1.1/batch_encoder/_bitrate_mode.py` & `animethemes-batch-encoder-1.2/batch_encoder/_bitrate_mode.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.1/batch_encoder/_colorspace.py` & `animethemes-batch-encoder-1.2/batch_encoder/_colorspace.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.1/batch_encoder/_encode_webm.py` & `animethemes-batch-encoder-1.2/batch_encoder/_encode_webm.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                f'-c:v libvpx-vp9 ' \
                f'{encoding_mode.second_pass_rate_control(self.cbr_bitrate, self.cbr_max_bitrate, crf)} ' \
                f'-cpu-used 0 -g {self.g} -threads {threads} {self.get_audio_filters()}{video_filters} -tile-columns 6 ' \
                f'-frame-parallel 0 -auto-alt-ref 1 -lag-in-frames 25 -row-mt 1 -pix_fmt yuv420p ' \
                f'{self.colorspace.get_args()} ' \
                f'-c:a libopus -b:a {self.audio_bitrate} -ar 48k ' \
                f'{limit_size}' \
-               f'-map_metadata -1 -map_chapters -1 -sn -f webm -y {webm_filename}.webm'
+               f'-map_metadata:g -1 -map_metadata:s:v -1 -map_metadata:s:a -1 -map_chapters -1 -sn -f webm -y {webm_filename}.webm'
 
     # Build audio filtergraph for encodes
     def get_audio_filters(self):
         audio_filters = []
         self.source_file.apply_audio_resampling(audio_filters)
         audio_filters.append(self.loudnorm_filter.get_normalization_filter())
         return '-af ' + ','.join(audio_filters)
```

### Comparing `animethemes-batch-encoder-1.1/batch_encoder/_encoding_config.py` & `animethemes-batch-encoder-1.2/batch_encoder/_encoding_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,39 +4,42 @@
 class EncodingConfig:
     # Config keys
     config_allowed_filetypes = 'AllowedFileTypes'
     config_encoding_modes = 'EncodingModes'
     config_crfs = 'CRFs'
     config_threads = 'Threads'
     config_limit_size_enable = 'LimitSizeEnable'
+    config_alternate_source_files = 'AlternateSourceFiles'
     config_include_unfiltered = 'IncludeUnfiltered'
 
     # Default Config keys
     config_default_video_stream = 'DefaultVideoStream'
     config_default_audio_stream = 'DefaultAudioStream'
 
     # Default config values
     default_allowed_filetypes = '.avi,.m2ts,.mkv,.mp4,.wmv'
     default_encoding_modes = f'{BitrateMode.VBR.name},{BitrateMode.CBR.name}'
     default_crfs = '12,15,18,21,24'
-    default_limit_size_enable = True
     default_threads = '4'
+    default_limit_size_enable = True
+    default_alternate_source_files = False
     default_include_unfiltered = True
     default_video_filters = {'filtered': 'hqdn3d=0:0:3:3,gradfun,unsharp',
                              'lightdenoise': 'hqdn3d=0:0:3:3',
                              'heavydenoise': 'hqdn3d=1.5:1.5:6:6',
                              'unsharp': 'unsharp'}
 
-    def __init__(self, allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, include_unfiltered, video_filters, default_video_stream,
+    def __init__(self, allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, alternate_source_files, include_unfiltered, video_filters, default_video_stream,
                  default_audio_stream):
         self.allowed_filetypes = allowed_filetypes
         self.encoding_modes = encoding_modes
         self.crfs = crfs
         self.threads = threads
         self.limit_size_enable = limit_size_enable
+        self.alternate_source_files = alternate_source_files
         self.include_unfiltered = include_unfiltered
         self.video_filters = video_filters
         self.default_video_stream = default_video_stream
         self.default_audio_stream = default_audio_stream
 
     @classmethod
     def from_config(cls, config):
@@ -44,22 +47,23 @@
                                                    EncodingConfig.default_allowed_filetypes).split(',')
         encoding_modes = config['Encoding'].get(EncodingConfig.config_encoding_modes,
                                                 EncodingConfig.default_encoding_modes).split(',')
         crfs = config['Encoding'].get(EncodingConfig.config_crfs, EncodingConfig.default_crfs).split(',')
         threads = config['Encoding'].get(EncodingConfig.config_threads,
                                          EncodingConfig.default_threads)
         limit_size_enable = config.getboolean('Encoding', EncodingConfig.config_limit_size_enable, fallback=EncodingConfig.default_limit_size_enable)
+        alternate_source_files = config.getboolean('Encoding', EncodingConfig.config_alternate_source_files, fallback=EncodingConfig.default_alternate_source_files)
         include_unfiltered = config.getboolean('Encoding', EncodingConfig.config_include_unfiltered,
                                                fallback=EncodingConfig.default_include_unfiltered)
         video_filters = config.items('VideoFilters', EncodingConfig.default_video_filters)
 
         default_video_stream = config['Encoding'].get(EncodingConfig.config_default_video_stream)
         default_audio_stream = config['Encoding'].get(EncodingConfig.config_default_audio_stream)
 
-        return cls(allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, include_unfiltered, video_filters, default_video_stream,
+        return cls(allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, alternate_source_files, include_unfiltered, video_filters, default_video_stream,
                    default_audio_stream)
 
     def get_default_stream(self, stream_type):
         if stream_type == 'video':
             return self.default_video_stream
         elif stream_type == 'audio':
             return self.default_audio_stream
```

### Comparing `animethemes-batch-encoder-1.1/batch_encoder/_loudnorm_filter.py` & `animethemes-batch-encoder-1.2/batch_encoder/_loudnorm_filter.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.1/batch_encoder/_seek.py` & `animethemes-batch-encoder-1.2/batch_encoder/_seek.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.1/batch_encoder/_seek_collector.py` & `animethemes-batch-encoder-1.2/batch_encoder/_seek_collector.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.1/batch_encoder/_source_file.py` & `animethemes-batch-encoder-1.2/batch_encoder/_source_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,8 +146,8 @@
                 logging.error('Please respond with \'y\' or \'n\'')
 
     # If our source file audio stream is not a 2-channel stereo layout, we need to resample it before normalization
     def apply_audio_resampling(self, audio_filters):
         channels = int(self.audio_format['streams'][0].get('channels', 2))
         channel_layout = self.audio_format['streams'][0].get('channel_layout', 'stereo')
         if channels != 2 or channel_layout != 'stereo':
-            audio_filters.append('aresample=ocl=stereo')
+            audio_filters.append('aresample=ochl=stereo')
```

### Comparing `animethemes-batch-encoder-1.1/batch_encoder/_utils.py` & `animethemes-batch-encoder-1.2/batch_encoder/_utils.py`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.1/setup.py` & `animethemes-batch-encoder-1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='animethemes-batch-encoder',
-    version='1.1',
+    version='1.2',
     author='AnimeThemes',
     author_email='admin@animethemes.moe',
     url='https://github.com/AnimeThemes/animethemes-batch-encoder',
     description='Generate/Execute FFmpeg commands for files in acting directory',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

