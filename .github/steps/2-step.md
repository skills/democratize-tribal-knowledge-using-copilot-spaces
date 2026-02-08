## Step 2: Explore & summarize project management processes and create a README

In this step you will:

- Explore the process docs in the docs/ folder (e.g., project-lifecycle.md, roles-responsibilities.md, communication-plan.md)
- Generate a 3–4 paragraph summary in your Copilot Space (workflows, roles, communication, quality)
- Use that summary to create/attach the existing issue about the README
- Create a pull request adding a README that links all process docs and includes the brief overview

### 📖 Theory: Attaching issues and assigning to the GitHub Copilot coding agent

While reading, note:

- End-to-end workflow stages and handoffs
- Defined roles/personas and responsibilities
- Decision / escalation points
- Communication cadences and channels
- Quality gates, reviews, and acceptance criteria

You will use the prompts below to:

1. Summarize the docs
2. Attach the prior issue
3. Generate a PR adding a docs/ README with links + overview

Proceed to the activities and run the provided prompts in your Copilot Space.

### ⌨️ Activity: Explore the project management process docs and Summarize in your Copilot Space

- Generate a summary. Should be 3-4 paragraphs covering the main processes OctoAcme uses for project management.
- Open your Copilot Space you created in the previous step. https://github.com/copilot/spaces or by clicking the name <img width="50%" height="50%" alt="link to Copilot Space" src="https://github.com/user-attachments/assets/13534299-c764-4d20-9760-88bd7dac7cff" />
- Start a new conversation in the Copilot Space and prompt the following:
  <img width="70%" height="70%" alt="Copilot Space conversation OctoAcme project management process docs summary" src="https://github.com/user-attachments/assets/342605be-4b36-48b2-b54f-18ae85f16bb8" />

  > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
  >
  > ```prompt
  > - Create a 3-4 paragraph summary of the project management processes used by OctoAcme
  >   based on the documentation in the docs folder of this repository.
  > - Focus on key workflows, personas/roles, communication strategies, and quality assurance practices.
  > ```

<details>
<summary> 📷 Show screenshot of the conversation output</summary>

<img width="50%" height="50%" alt="Copilot response with the summary" src="https://github.com/user-attachments/assets/26a54642-a14b-498d-a195-d1ffd45e5679" />

</details>

### ⌨️ Activity: Attach an issue and create a pull request for the Copilot coding agent

In this activity, you will connect the issue you created in Step 1 to your Copilot Space conversation and use the coding agent to automatically create a pull request.

1. **Find your issue number**: Go to [https://github.com/{{full_repo_name}}/issues](https://github.com/{{full_repo_name}}/issues) and note the issue number from Step 1 (it should be about creating a README for project management docs)

1. **Attach the issue to your conversation**: In your Copilot Space, type the following (replace `#` with your actual issue number):

> [!IMPORTANT]
> After typing the issue reference below, press **\<SHIFT\> + \<ENTER\>** to add it to the conversation without sending the message yet.

```text
@{{full_repo_name}}/issues/#
```

(Example: if your issue is #2, type `@{{full_repo_name}}/issues/2`)

1. **Verify the issue is attached**: You should see the issue title and details appear in your conversation

1. **Create the pull request**: Now send this prompt to create the pull request:

   <img width="80%" height="80%" alt="repository issue and pull request creation" src="https://github.com/user-attachments/assets/af469c6a-fc87-454b-9a65-23ffe0d7cd50" />
   
   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
   >
   > ```prompt
   > - Using the github-coding-agent tool create a pull request based on the attached issue.
   > - The README should also contain a brief overview of the project management processes
   >   used by OctoAcme based on the summary we just created.
   > - The README should be in the `docs/` folder
   > - Add this pull request to the attached issue.
   > - Add {{login}} as a reviewer for the pull request
   > ```

1. **Allow the coding agent**: When prompted, select **Allow** to let the coding agent work on your repository

   <img width="50%" height="50%" alt="Copilot coding agent allow" src="https://github.com/user-attachments/assets/b0c92c04-d12b-4c5e-b682-33643b90ee11" />

1. **Monitor progress**: You should receive a notification that the Copilot coding agent is working on your pull request.

   There are two ways you can check the status of the coding agent working on your pull request
   1. Go to your repository and click **Pull requests** to see the progress:

      <img width="70%" height="70%" alt="pull requests" src="https://github.com/user-attachments/assets/88e9876e-2dae-43a4-86ff-29c4cdc6077c" />

   1. You can track progress and view details in **Mission Control** for **agent tasks** by following the task link

      <img width="40%" height="40%" alt="mission control" src="https://github.com/user-attachments/assets/a64c1826-720e-4b5f-8d0f-8aebc9aca501" />

1. **Check open pull requests**: We can check pull request status from our **Copilot Space** as well.

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
   >
   > ```prompt
   > check open pull requests
   > ```

   <img width="40%" height="40%" alt="mission control" src="https://github.com/user-attachments/assets/ef0ffd8a-ba8f-4618-a2cc-8e1e0d1bb309" />

> [!NOTE]  
> The coding agent typically takes 5-15 minutes to complete the work. You can click **View session** to watch the progress if desired.

1. **Review and merge**: Once the pull request is ready:

   a. **Submit review**: Leave a comment (optional), click **Approve**, then **Submit review**

      <img width="70%" height="70%" alt="Add review" src="https://github.com/user-attachments/assets/ea460dc3-a86d-467b-8469-bd9244b915ea" />

      <img width="50%" height="50%" alt="Submit review" src="https://github.com/user-attachments/assets/15042891-c8fa-4acc-a25d-c588cf6a3ffe" />

   b. **Merge**: Select **Ready for review**, then **Merge pull request** and **Confirm merge**

      <img width="50%" height="50%" alt="Ready for review" src="https://github.com/user-attachments/assets/2348378d-a597-404f-827d-4003d79055c0" />
      <img width="50%" height="50%" alt="Merge pull request" src="https://github.com/user-attachments/assets/fda15799-a123-4e6a-b32a-c7ec44db3418" />

<details>
<summary>Having trouble? 🤷</summary>

- **Can't find your issue?** Check the [Issues tab](https://github.com/{{full_repo_name}}/issues) in your repository for the issue you created in Step 1
- **Issue not attaching?** Make sure you're using the exact format `@{{full_repo_name}}/issues/#` where `#` is your issue number
- **Coding agent not working?** Ensure you have the necessary permissions to create pull requests in your repository
- **Pull request creation failed?** The issue must be properly attached before the coding agent can work on it

</details>
