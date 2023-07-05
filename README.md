# ChatGPT Console Application

This is a console application that allows you to chat with ChatGPT using the OpenAI GPT-3.5 language model. The application prompts you to enter your concerns or questions, and it generates responses using the ChatGPT model.

## Prerequisites

Before running the application, make sure you have the following prerequisites:

- Go programming language (version 1.16 or later) installed on your machine.
- Access to the OpenAI GPT-3.5 API.

## Installation

To install the required dependencies, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/your-repo/chatgpt-console.git
   ```

2. Change into the project directory:

   ```bash
   cd chatgpt-console
   ```

3. Install the dependencies using Go modules:

   ```bash
   go mod download
   ```

## Configuration

The application requires an API key to access the OpenAI GPT-3.5 API. Follow these steps to configure the API key:

1. Rename the `.env.example` file to `.env`.

2. Open the `.env` file in a text editor.

3. Replace the placeholder value with your actual API key:

   ```
   API_KEY=your-api-key
   ```

## Usage

To use the application, follow these steps:

1. Open a terminal or command prompt.

2. Navigate to the project directory.

3. Run the application:

   ```bash
   go run main.go
   ```

4. The application will prompt you to enter your concerns or questions. Type your input and press Enter.

5. The application will generate a response from ChatGPT and display it in the console.

6. Repeat steps 4-5 to continue the conversation. To end the conversation, type `quit` and press Enter.

## Customization

You can modify the application to suit your needs. Here are some possible customizations:

- Change the ChatGPT engine: By default, the application uses the `gpt3.TextDavinci003Engine` engine. You can explore other available engines provided by the `go-gpt3` package and modify the `GetResponse` function to use a different engine.

- Adjust the response parameters: The `GetResponse` function accepts various parameters for generating responses, such as `MaxTokens` and `Temperature`. You can modify these parameters to control the length and randomness of the generated responses.

## Limitations

Keep in mind the following limitations of the application:

- The quality of responses depends on the training of the ChatGPT model and the provided input. The model may not always generate accurate or desired responses.

- The application uses the OpenAI GPT-3.5 API, which may have usage limits and cost implications. Make sure to review the OpenAI documentation for more information on API usage and pricing.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code according to your needs.
