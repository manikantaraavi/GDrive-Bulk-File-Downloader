# GDrive-Bulk-File-Downloader 📁 🔗

This script, designed for use within Google Colab, downloads files from a specified Google Drive folder and organizes them into zip archives on your Google Drive. 

## Features ✨

* Downloads all files (with focus on video) from a given Google Drive folder. 📥
* Automatically splits downloads into multiple zip archives to manage large file sizes. 📦
* Provides progress updates during the download and zipping process. 🔄
* Stores the downloaded zip archives in a specified folder on your Google Drive. 💾

## How to Use 🚀

1. **Replace Placeholders:** 
    * In the code, you'll need to replace `folder_id` with the actual ID of your Google Drive folder containing the files. 
    * You should also modify `zip_destination_base_path` to specify the desired location on your Google Drive where the zip archives will be saved. 
2. **Run the Code:** Execute the script in your Google Colab environment. ▶️
3. **Authenticate:** You'll be prompted to authenticate your Google account to access Google Drive. 🔑
4. **Download and Zip:** The script will download the files and automatically create zip archives. 📥 📦


## Data to Replace 📝

*  `folder_id`:  Replace `'1xHOwL-cn_yjSVOZolt69VDCpYSlcszIn'` with the ID of your Google Drive folder. You can find the folder ID in the URL of the folder when you open it in your browser.
*  `zip_destination_base_path`:  Change `"/gdrive/MyDrive/Downloaded_Videos"` to your preferred location on Google Drive for saving the zip files.


## Summary for Non-Coders 👶

Imagine you have a folder in your Google Drive full of files (primarily videos). This script, running in Google Colab, acts like a helpful robot:

1. It connects to your Google Drive. 🔗
2. It finds all the files in your specified folder. 🔎
3. It downloads them one by one. 📥
4. It neatly packs groups of files into zip files, like putting clothes into suitcases. 🧳
5. It saves these zip files back to your Google Drive in a location you choose. 💾

This way, you can easily download and organize many files from your Google Drive.


## Disclaimer ⚠️

This code is provided as-is and without warranty. Use it at your own risk. Please ensure you have the necessary permissions to access and download the files in the specified Google Drive folder. 

## Potential Improvements 📈

* Add error handling for network issues or invalid folder IDs. ❌
* Allow users to customize the number of files per zip archive through an input. 🔢
* Implement a mechanism to resume interrupted downloads. ⏯️
