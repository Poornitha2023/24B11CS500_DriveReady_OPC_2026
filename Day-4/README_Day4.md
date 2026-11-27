# Day 4 -- LangChain, Conversation Memory and AI Agents

## Project: Campus Stationery & Print Hub Assistant

### Overview

This project is a simple AI-powered Stationery and Print Hub Assistant
developed using Python, LangChain, and the Groq API. It helps customers
check stationery and printing prices, view shop opening hours, and place
orders for notebooks, black-and-white printing, and spiral binding.

The assistant uses LangChain tools to calculate prices, check opening
hours, and save confirmed orders to Google Sheets. It also maintains
conversation history so it can follow the conversation across multiple
messages.

This task demonstrates important concepts of LangChain, chat models, AI
agents, tool calling, conversation memory, Pydantic data validation,
Python functions, and Google Sheets integration.

### Technologies Used

-   Python
-   Google Colab
-   Groq API
-   LangChain
-   LangChain Groq
-   Pydantic
-   Google Sheets
-   `gspread`
-   Google Colab Secrets and Google authentication

### Concepts Covered

1.  **LangChain Integration:** Connecting the Groq language model using
    LangChain.
2.  **Chat Models:** Using `ChatGroq` to interact with the Groq language
    model.
3.  **AI Agents:** Creating an agent using LangChain's `create_agent`.
4.  **Tool Calling:** Giving the agent tools to calculate prices, check
    opening hours, and save orders.
5.  **Conversation Memory:** Maintaining conversation history so the
    assistant can use details shared in earlier messages.
6.  **Pydantic Validation:** Defining an order model with required
    fields, allowed item choices, and quantity validation.
7.  **Python Functions:** Creating reusable tools with the `@tool`
    decorator and type hints.
8.  **Google Sheets Integration:** Saving confirmed customer orders in a
    Google Sheet.
9.  **Error Handling:** Handling invalid order details and errors during
    agent execution.
10. **Prompt Instructions:** Defining the assistant's role, business
    information, tool-use rules, and response style in a system prompt.

### Features

-   Provides prices for notebooks, black-and-white printing, and spiral
    binding.
-   Calculates the total cost based on the requested quantity.
-   Checks shop opening hours for each day of the week.
-   Collects customer details before saving an order.
-   Asks whether printing should be double-sided.
-   Saves confirmed orders to Google Sheets.
-   Maintains conversation history.
-   Supports friendly English or Telugu responses.
-   Handles invalid order details and agent errors.

### How to Run

1.  Open the `AI_Agent_Updated.ipynb` notebook in Google Colab.
2.  Run the package installation cell.
3.  Add your Groq API key to Colab Secrets with the name `GROQ_API_KEY`.
4.  Run the Google authentication and Google Sheets setup cell.
5.  Complete Google account authorization when prompted.
6.  Run the remaining notebook cells sequentially.
7.  Chat with the assistant to check prices, shop hours, or place an
    order.

**Note:** The notebook creates a Google Sheet named
`Campus Stationery Orders`. Run the setup cell only when you want to
create a new sheet. If you rerun the notebook in a new session and want
to continue using an existing sheet, open that sheet with `gspread`
instead of creating another one.

### Sample Questions

-   How much does one notebook cost?
-   What is the price for 20 black-and-white print pages?
-   Is the shop open on Sunday?
-   What are your Saturday opening hours?
-   I'm Ravi. I need 3 notebooks for pickup on 2 December.
-   My name is Anu. Please print 80 pages double-sided for pickup on 3
    December.
-   How much will 5 spiral binding jobs cost?
-   Can I place an order for 2 notebooks?

### Learning Outcome

Through this task, I learned how to build a conversational AI assistant
using Python, LangChain, and Groq. I understood how an AI agent uses
tools to perform tasks, how conversation history helps maintain context,
how Pydantic validates order details, and how Google Sheets can be used
to store customer orders.

------------------------------------------------------------------------

**Task:** Day 4 -- Agentic AI Learning\
**Project:** Campus Stationery & Print Hub Assistant
