# Helkor upload

This action uploads a zip file, extracts it and restarts the server.

## Usage

### Variables
- `SERVER_ID` - ID of the server you want to upload to. You can find it in the URL when you are in the server detail page.
- `AUTH_TOKEN` - Your auth token for the Helkor API for the account you want to use to upload with. You can find it in your account settings.
- `FTP_PASSWORD` - Your FTP password. It is the same as the password to your Helkor account.
- `FOLDER_TO_ZIP` - The folder you want to zip and upload.
- `ZIP_FILE_NAME` - The name of the zip file you want to upload. The default name is "code.zip".
- `UPLOAD_PATH` - The path where you want to upload the zip file. The default path is the root folder.
