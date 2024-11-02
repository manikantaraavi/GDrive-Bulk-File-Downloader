# GDrive-Bulk-File-Downloader 📁 🔗

This script, designed for use within Google Colab, downloads files from a specified Google Drive folder and organizes them into zip archives on your Google Drive. This is particularly useful for backing up large amounts of data, like videos, from Google Drive to your local machine or another cloud storage service.

## Features ✨

* **Bulk Download:** Downloads all files from a given Google Drive folder, with a focus on video files. 📥
* **Zip Archiving:** Automatically splits downloads into multiple zip archives, making it easier to manage large file sizes. 📦
* **Progress Updates:** Provides real-time progress updates during the download and zipping process, keeping you informed about the status. 🔄
* **Organized Storage:** Stores the downloaded zip archives in a specified folder on your Google Drive, allowing for easy organization. 💾

## How to Use 🚀

1. **Set up Google Cloud Project and Credentials:**
   - To make this code work, you'll need a `credentials.json` file. If you don't know how to create one, just search on Google for instructions. You'll need to upload this file into the current Colab directory for the script to access it.
   - **Set the `GOOGLE_APPLICATION_CREDENTIALS` Environment Variable:** After uploading the JSON key file, you need to tell your Colab environment where to find it. This is done by setting the `GOOGLE_APPLICATION_CREDENTIALS` environment variable to the path of your credentials file. Use the following code snippet, replacing `/path/to/your/credentials.json` with the actual path to your uploaded JSON file:
   - **Important:** This environment variable is only set for the current Colab session. If you restart your runtime, you'll need to set it again.

2. **Replace Placeholders in the Code:** 

   - **`folder_id`:** Replace `'1xHOwL-cn_yjSVOZolt69VDCpYSlcszIn'` with the actual ID of the Google Drive folder you want to download files from. You can find the folder ID in the URL of the folder when you open it in your browser (it's the long string of characters after `/folders/`).
   - **`zip_destination_base_path`:** Change `"/gdrive/MyDrive/Downloaded_Videos"` to the desired location on your Google Drive where you want the downloaded zip archives to be saved. Make sure the folder exists.
   - **`/path/to/your/credentials.json`:** Double-check that this path in your code matches the actual path to your uploaded credentials JSON file.

3. **Run the Code:** Execute the script in your Google Colab environment by clicking the "Play" button on the code cell. ▶️

4. **Authenticate (if prompted):** If you haven't already authenticated using the JSON key file, you might be prompted to authenticate with your Google account. This usually happens if there's an issue with the credentials file or if you're using a different authentication method. 🔑

5. **Download and Zip:** The script will start downloading files from the specified folder and automatically create zip archives. You'll see progress updates in the output, indicating the download status and speed. 📥 📦


## Data to Replace 📝

*  **`folder_id`:**  Replace `'1xHOwL-cn_yjSVOZolt69VDCpYSlcszIn'` with the ID of your Google Drive folder. You can find the folder ID in the URL of the folder when you open it in your browser.
*  **`zip_destination_base_path`:**  Change `"/gdrive/MyDrive/Downloaded_Videos"` to your preferred location on Google Drive for saving the zip files.
*  `/path/to/your/credentials.json`: Replace with the path to your downloaded JSON credentials file.



## Summary for Non-Coders 👶

Imagine you have a folder in your Google Drive full of files (primarily videos). This script, running in Google Colab, acts like a helpful robot:

1. It connects to your Google Drive using special "credentials" (like a key). 🔑
2. It finds all the files in your specified folder. 🔎
3. It downloads them one by one. 📥
4. It neatly packs groups of files into zip files, like putting clothes into suitcases. 🧳
5. It saves these zip files back to your Google Drive
