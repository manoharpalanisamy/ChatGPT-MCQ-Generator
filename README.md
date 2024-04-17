# ChatGPT MCQ Generator

Effortlessly generate multiple-choice questions (MCQs) with the power of AI using the ChatGPT-3.5-turbo model.

## Project Description

The ChatGPT MCQ Generator is a modular project developed to generate multiple-choice questions based on user inputs and subject-specific data. Leveraging the OpenAI API, specifically the chatGPT-3.5-turbo model, along with Langchain and Streamlit UI, this project utilizes advanced natural language processing capabilities to analyze input data and generate relevant MCQs. The generated MCQs are presented in a user-friendly table format using Streamlit. Additionally, the project is deployed on AWS EC2 for seamless accessibility and scalability.

## Project Setup in Server

1. **Login to AWS:** Access the AWS Management Console at [https://aws.amazon.com/console/](https://aws.amazon.com/console/).
2. **Launch EC2 Instance:** Search for EC2 and configure an Ubuntu machine.
3. **Update the Machine:**
    ```bash
    sudo apt update
    sudo apt-get update
    sudo apt upgrade -y
    sudo apt install git curl unzip tar make sudo vim wget -y
    ```
4. **Clone Repository:**
    ```bash
    git clone https://github.com/send2manoo/ChatGPT-MCQ-Generator.git
    ```
5. **Install Dependencies:**
    ```bash
    sudo apt install python3-pip
    pip3 install -r requirements.txt
    ```
6. **Run Streamlit App:**
    ```bash
    python3 -m streamlit run StreamlitAPP.py
    ```
7. **Add OpenAI API Key (Optional):**
    - Create a `.env` file in your server: `touch .env`
    - Edit the `.env` file: `vi .env`
    - Copy your API key and paste it into the `.env` file.
    - Save and exit the editor: Press `Esc`, then `:wq`, and hit `Enter`.
8. **Configure Security:**
    - Navigate to security settings and add an inbound rule for port 8501.

---

This README provides a comprehensive guide for setting up and running the ChatGPT MCQ Generator project on an AWS EC2 instance. For more details on the project, including its features and usage, refer to the project documentation and codebase.
