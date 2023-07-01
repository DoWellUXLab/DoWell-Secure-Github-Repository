# DoWell Secure Github Repository


Welcome to the Secure Repository API!. This API seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The API offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository API ensures the integrity and availability of your code backups.

## Features

The Secure Repository API offers a range of powerful features to enhance code backup:

1. Repository Clone: The API enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.

2. Webhooks Integration: With seamless integration with Github's webhooks, the API automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the API captures these changes in real-time, ensuring that your backups are always up to date.

3. Backup Reports: The Secure Repository API generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.

4. Repository Reports: In addition to backup reports, the API also generates repository reports, offering an overview of each repository's status and health. These reports provide information such as the number of commits, branches, and contributors, giving you a clear snapshot of your codebase's activity and progress.

## Getting Started

Getting Started with the Secure Repository API's Key Features:

1. Review the [API Documentation](https://documenter.getpostman.com/view/27523601/2s93zB6N48) to understand the available endpoints, request parameters, and response formats.

2. To clone a repository using the Secure Repository API, make a POST request to the following endpoint: POST ```/repository-clone```. 
Include the following payload data in the request body:
    ```json
    {
        "repository_url": "<repository_url>",
        "api_key": "<api_key>",
        "services": "DoWell Secure Repository"
    }
    ```
    Replace the repository_url value with the URL of the repository you want to clone. Ensure you provide a valid api_key to authenticate your request. The services field indicates the service you want to utilize i.e "DoWell Secure Repository".

3. To set up a webhook for the Secure Repository API, follow the standard webhook creation process provided by Github. Configure the webhook's payload URL to point to url recieved from the repository-clone endpoint within your application to handle the backup events triggered by the webhook.

4. To retrieve backup reports using the Secure Repository API, send a GET request to the following endpoint: GET ```/backup-reports/<api_key>/```.
Replace <api_key> with the actual API key associated with your backups. This request will fetch the backup reports containing valuable information such as timestamps, repository names, and any encountered errors during the backup process.

5. To obtain repository reports through the Secure Repository API, issue a GET request to the following endpoint: GET ```/repository-reports/<api_key>/```.
Replace <api_key> with the appropriate API key linked to your repositories. This request will provide you with an overview of each repository's status, including details like commit count, branch information, and contributors.

## Documentation and Support

For detailed API documentation, including endpoint descriptions, request and response examples, and authentication details, please refer to the [API Documentation](https://documenter.getpostman.com/view/27523601/2s93zB6N48).

If you encounter any issues, have questions, or need assistance with the Secure Repository API, please contact our support team.
