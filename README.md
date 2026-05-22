# Rosetta Stone Lesson Finisher

This is a Node.js program designed to automatically complete lessons on the Rosetta Stone platform using network requests. It's useful for users who want to quickly finish lessons in a structured way, especially in an educational context. Please note that this program requires certain constants, such as authorization and session tokens, to work correctly. These tokens can be obtained through network requests when logging into the Rosetta Stone platform. Additionally, this can be run in browser as it uses no dependencies.

If you need assistance obtaining the required tokens, you can contact the program's author me on GitHub.

> This project is originally created by [Sam Pearlman](https://github.com/SamPearlma).
> The original repository is no longer available, so this version serves as a backup to preserve the code.
> Some accompanying guide videos were also recreated for reference.

## Note

This script only works with Rosetta Stone Foundations (A1–A2 levels).

If you are using Rosetta Stone Fluency Builder (B1–C1 levels), you should instead use the browser extension [RosettaStonks](https://github.com/m1dugh/RosettaStonks), which is easier to use and is also expected to work with Foundations.

## Configuration

To configure the program, open the constants.json file and set the following constants:

```json
{
  "person": "YOUR_NAME (Not Required)",
  "authorization": "YOUR_AUTHORIZATION_TOKEN",
  "sessionToken": "YOUR_SESSION_TOKEN",
  "schoolName": "YOUR_SCHOOL_NAME",
  "unitsToComplete": [1, 2, 3], // Replace with the unit numbers you want to complete
  "userId": "YOUR_USER_ID",
  "languageCode": "YOUR_LANGUAGE_CODE" // E.g., "HEB" for Hebrew, "FRA" for French, etc.
}
```

Make sure to replace `YOUR_AUTHORIZATION_TOKEN`, `YOUR_SESSION_TOKEN`, `YOUR_SCHOOL_NAME`, `YOUR_USER_ID`, and `YOUR_LANGUAGE_CODE` with your actual Rosetta Stone credentials.

> The required values are explained in [Filling Constants.json](#filling-constantsjson).

## Usage

TO BEGIN
Make sure to install nodejs from here https://nodejs.org.

### Download files

This is a video showing how to download the files from github and open the ones you need in a text editor

https://github.com/user-attachments/assets/4fc7014e-6d78-44fc-a8a0-54e17e9c0b6f

### Filling Constants.json

https://github.com/user-attachments/assets/907f2c0d-22b6-4f1f-9901-13e8c7469d0e

### Percent Correct (OPTIONAL)

By default, the program randomly does between 89% to 100% correct. If you want to change it follow this video

https://github.com/user-attachments/assets/dc81d623-0062-4008-9620-8e75e79464ef

### Running program

This video shows you how to run the program

https://github.com/user-attachments/assets/3f38a70d-d4b3-4348-ba8d-8cbbdc5e8c63

## Program Files

- index.js: The main program file that orchestrates the lesson completion process.
- getData.js: This file retrieves necessary data from the Rosetta Stone platform using network requests.
- makeRequest.js: Handles making network requests to mark lessons as completed.

## Disclaimer

Use this program responsibly and in accordance with Rosetta Stone's terms and conditions. Automated completion of lessons may violate their policies. The I take no responsibility for any misuse or consequences that may arise from using this software.
