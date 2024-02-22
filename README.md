# GitHub Unfollow in Go

This Go script automatically unfollows users on GitHub who do not follow you back, with the option to maintain a whitelist of users that you do not want to unfollow.

## Installation

To use this script, you need to have Go installed. If you do not have Go installed, you can download it from [golang.org](https://golang.org/dl/).

Once Go is installed, clone this repository to your local machine with the following command:

    git clone git@github.com:thiagopac/github-unfollow-go.git

    cd github-unfollow-go

## Creating a Personal Access Token

To authenticate with the GitHub API, you will need to create a Personal Access Token. Follow these steps to create one:

1. Go to your GitHub account settings.

2. Scroll down to the **Developer settings** section and select **Personal access tokens**.

3. Click on the **Generate new token** dropdown and select **Generate new token (classic)**.

4. Give your token a descriptive name.

5. In the **Select scopes** section, ensure that you check the `user` > `user:follow` permission to allow the script to manage following and unfollowing.

6. Once the token is created, make sure to copy it to your clipboard.

**Important:** Treat your tokens like passwords and keep them secret. Do not share your tokens in public spaces, and do not include them in your repository.

## Usage

To run the script, use the following command in the terminal, replacing `<YOUR-TOKEN>` with the Personal Access Token you generated and `user1 user2 user3` with the GitHub usernames you want to keep following (your whitelist):

    go run . <YOUR-TOKEN> user1 user2 user3

The script will unfollow users who do not follow you back, except for the ones listed in the whitelist.

## Contributing

Contributions to this project are welcome. You can contribute by:

- Suggesting new features

- Submitting pull requests

## License

This project is licensed under the [ISC License](LICENSE.md).

## All script languages

- [GitHub Unfollow in JavaScript](https://github.com/thiagopac/github-unfollow)
- [GitHub Unfollow in TypeScript](https://github.com/thiagopac/github-unfollow-ts)
- [GitHub Unfollow in Go](https://github.com/thiagopac/github-unfollow-go)
- [GitHub Unfollow in Go](https://github.com/thiagopac/github-unfollow-py)
