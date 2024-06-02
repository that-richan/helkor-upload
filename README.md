# Helkor upload

This action uploads a zip file, extracts it and restarts the server.

## Usage

### Variables
- `SERVER_ID` - ID of the server you want to upload to. You can find it in the URL when you are in the server detail page.
- `AUTH_TOKEN` - Your auth token for the Helkor API for the account you want to use to upload with. You can find it in your account settings.
- `FTP_PASSWORD` - Your FTP password. It is the same as the password to your Helkor account.
- `FOLDER_TO_ZIP` - The folder you want to zip and upload.
- `ZIP_FILE_NAME` - Custom name of the zip file you want to upload. The default name is "code.zip".
- `UPLOAD_PATH` - Custom path where you want to upload and extract the zip file. The default path is the root folder.

## Example

```yaml
- name: Upload to helkor
  uses: that-richan/action-upload@latest
  with:
    SERVER_ID: '123456'
    AUTH_TOKEN: ${{ secrets.AUTH_TOKEN }} # Please, set & store your credentials/API keys in GitHub secrets
    FTP_PASSWORD: ${{ secrets.FTP_PASSWORD }} # Please, set & store your credentials/API keys in GitHub secrets
    FOLDER_TO_ZIP: 'build'
```
