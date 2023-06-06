# Comparing `tmp/video2image-1.2.0.tar.gz` & `tmp/video2image-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video2image-1.2.0.tar", last modified: Tue Jun  6 16:11:39 2023, max compression
+gzip compressed data, was "video2image-1.3.0.tar", last modified: Tue Jun  6 17:29:04 2023, max compression
```

## Comparing `video2image-1.2.0.tar` & `video2image-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:11:39.695147 video2image-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-06 16:11:29.000000 video2image-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 16:11:39.695147 video2image-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-06 16:11:29.000000 video2image-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 16:11:39.695147 video2image-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-06 16:11:29.000000 video2image-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:11:39.695147 video2image-1.2.0/video2image/
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-06 16:11:29.000000 video2image-1.2.0/video2image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-06 16:11:29.000000 video2image-1.2.0/video2image/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:11:39.695147 video2image-1.2.0/video2image.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 16:11:39.000000 video2image-1.2.0/video2image.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-06 16:11:39.000000 video2image-1.2.0/video2image.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:11:39.000000 video2image-1.2.0/video2image.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-06 16:11:39.000000 video2image-1.2.0/video2image.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 16:11:39.000000 video2image-1.2.0/video2image.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 16:11:39.000000 video2image-1.2.0/video2image.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:29:04.033719 video2image-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-06 17:28:54.000000 video2image-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 17:29:04.033719 video2image-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-06 17:28:54.000000 video2image-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:29:04.033719 video2image-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-06 17:28:54.000000 video2image-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:29:04.033719 video2image-1.3.0/video2image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-06 17:28:54.000000 video2image-1.3.0/video2image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-06 17:28:54.000000 video2image-1.3.0/video2image/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:29:04.033719 video2image-1.3.0/video2image.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 17:29:03.000000 video2image-1.3.0/video2image.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-06 17:29:04.000000 video2image-1.3.0/video2image.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:29:03.000000 video2image-1.3.0/video2image.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-06 17:29:03.000000 video2image-1.3.0/video2image.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 17:29:03.000000 video2image-1.3.0/video2image.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 17:29:03.000000 video2image-1.3.0/video2image.egg-info/top_level.txt
```

### Comparing `video2image-1.2.0/LICENSE` & `video2image-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `video2image-1.2.0/README.md` & `video2image-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # video2image
 Video2Image is a Python script that extracts frames from a video file or a set of video files and saves them as individual images. It provides a simple and convenient way to convert videos into a series of images. This can be useful for various applications such as computer vision, machine learning, data analysis, and more.
 
+https://pypi.org/project/video2image/
+
 ## Installation
 
 You can install Video2Image using `pip`. Here are the steps to install it:
 
 1. Open a terminal or command prompt.
 
 2. Run the following command to install the package:
```

### Comparing `video2image-1.2.0/video2image/__init__.py` & `video2image-1.3.0/video2image/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 
 def main():
     parser = argparse.ArgumentParser(description="Extract frames from video file(s)")
     parser.add_argument("-i", "--input", required=True, help="Path to the input video file or directory")
     parser.add_argument("-o", "--output", default="", help="Path to the output directory\n"
                                                            "(default: create a directory with the same name as the input video in the input directory)")
     parser.add_argument("-p", "--parent", action="store_true", help="Include the parent directory of the video in the output directory path")
-    parser.add_argument("-H", "--show-help", action="help", help="Show this help message and exit")  # Modified option string
+    parser.add_argument("-H", "--show-help", action="help", help="Show this help message and exit")
+    parser.add_argument("-f", "--format", default="jpg", choices=["jpg", "png"], help="Image format for extracted frames (default: jpg)")
     args = parser.parse_args()
     
     # Use input video directory as output if -o is empty
     if args.output == "":
         args.output = os.path.dirname(args.input)
     
     # Handle single video file
     if os.path.isfile(args.input):
-        extract_frames(args.input, args.output, args.parent)
+        extract_frames(args.input, args.output, args.parent, args.format)
     
     # Handle directory with multiple video files
     elif os.path.isdir(args.input):
         video_files = glob.glob(os.path.join(args.input, "*.mp4"))
         if len(video_files) == 0:
             print("No video files found in the input directory")
         else:
             for video_file in video_files:
-                extract_frames(video_file, args.output, args.parent)
+                extract_frames(video_file, args.output, args.parent, args.format)
     
     else:
         print("Invalid input: not a file or directory")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `video2image-1.2.0/video2image/converter.py` & `video2image-1.3.0/video2image/converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,71 @@
 import os
 import cv2
 import shutil
+from tqdm import tqdm
 
-def extract_frames(video_path, output_folder, include_parent=False):
+def extract_frames(video_path, output_folder, include_parent=False, image_format="jpg"):
     # Create the output folder if it doesn't exist
     os.makedirs(output_folder, exist_ok=True)
-    
+
     # Get the video file name without extension
     video_name = os.path.splitext(os.path.basename(video_path))[0]
-    
+
     if include_parent:
         # Include the parent directory in the output folder path
         parent_folder = os.path.dirname(video_path)
         frame_folder = os.path.join(output_folder, os.path.basename(parent_folder), video_name)
     else:
         # Create a folder for the video frames directly in the output folder
         frame_folder = os.path.join(output_folder, video_name)
-    
+
     if os.path.exists(frame_folder):
         # If the folder already exists, remove it and create again
         shutil.rmtree(frame_folder)
     os.makedirs(frame_folder)
-    
+
     # Open the video file
     video = cv2.VideoCapture(video_path)
-    
+
     # Check if video file opened successfully
     if not video.isOpened():
         print(f"Error opening video file: {video_path}")
         return
-    
-    # Initialize variables
-    frame_count = 0
-    
+
+    # Get video details
+    fps = video.get(cv2.CAP_PROP_FPS)
+    frame_count = int(video.get(cv2.CAP_PROP_FRAME_COUNT))
+    video_format = video.get(cv2.CAP_PROP_FORMAT)
+    video_size = (int(video.get(cv2.CAP_PROP_FRAME_WIDTH)), int(video.get(cv2.CAP_PROP_FRAME_HEIGHT)))
+
+    print(f"Video Details:")
+    print(f"  Format: {video_format}")
+    print(f"  Size: {video_size}")
+    print(f"  FPS: {fps}")
+    print(f"  Frame Count: {frame_count}")
+
+    # Set up progress bar
+    progress_bar = tqdm(total=frame_count, desc="Extracting Frames", unit="frame")
+
     while True:
         # Read the next frame from the video
         ret, frame = video.read()
-        
+
         # If frame reading was not successful, break the loop
         if not ret:
             break
-        
+
         # Save the frame as an image
-        frame_path = os.path.join(frame_folder, f"frame_{frame_count:04d}.jpg")
+        frame_path = os.path.join(frame_folder, f"frame_{frame_count:04d}.{image_format}")
         cv2.imwrite(frame_path, frame)
-        
-        # Increment frame count
-        frame_count += 1
-    
+
+        # Update progress bar
+        progress_bar.update(1)
+
+        # Decrement frame count
+        frame_count -= 1
+
     # Release the video object
     video.release()
-    
-    print(f"Frames extracted: {frame_count}")
+
+    # Close progress bar
+    progress_bar.close()
```

