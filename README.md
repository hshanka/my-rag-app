## Setup

This project requires an OpenAI API key to work. You need to create your own API key on [OpenAI's website](https://platform.openai.com) and then provide it to the application.

### How to Run the Application with Docker

Build the Docker image:
```bash
docker build -t my-rag-app .

### Run the Docker container while setting the API key as an environment variable:
docker run -it --rm -e OPENAI_API_KEY="your_openai_api_key_here" my-rag-app

---

### 3. Benefits

- **Security:**  
  Avoids exposing your private API key in the code or repository.

- **Flexibility:**  
  Each user can set their own API key, which is especially important because API keys are tied to individual accounts and usage limits.

- **Portability:**  
  Makes your project more portable and easier to share publicly since sensitive credentials are not included in the source code.

---

By following these steps, you ensure that the API key is externalized and securely provided at runtime. Anyone who downloads your project will need to obtain their own OpenAI API key and set it via the `OPENAI_API_KEY` environment variable before running the application.
