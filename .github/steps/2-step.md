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

> [!IMPORTANT]
> If you are using a Copilot free plan or are concerned with impacting premium usage quotas, use a **0x** model or **Auto** if available. These models do not consume premium request units. For more information, see [GitHub Copilot plans](https://docs.github.com/en/copilot/get-started/plans#comparing-copilot-plans) and [Copilot Requests](https://docs.github.com/en/copilot/concepts/billing/copilot-requests).

### ⌨️ Activity: Explore the project management process docs and Summarize in your Copilot Space

1. Generate a summary. Should be 3-4 paragraphs covering the main processes OctoAcme uses for project management.

   Open your Copilot Space you created in the previous step. https://github.com/copilot/spaces and select **Yours** and select **"OctoAcme Project Management Hub"**

   <img width="50%" alt="copilot-spaces-yours" src="../images/copilot-spaces-yours.png" />

2. Start a new conversation in the Copilot Space and prompt the following:

   <img width="70%" alt="copilot-spaces-conversation-summary" src="../images/copilot-spaces-conversation-summary.png" />

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
   >
   > ```prompt
   > - Create a 3-4 paragraph summary of the project management processes used by OctoAcme
   >   based on the documentation in the docs folder of this repository.
   > - Focus on key workflows, personas/roles, communication strategies, and quality assurance practices.
   > ```

   <details>
   <summary> 📷 Show screenshot of the conversation output</summary>

   <img width="50%" alt="copilot-spaces-conversation-summary-output" src="../images/copilot-spaces-conversation-summary-output.png" />

   </details>

### ⌨️ Activity: Attach an issue and create a pull request for the Copilot coding agent

In this activity, you will connect the issue you created in Step 1 to your Copilot Space conversation and use the coding agent to automatically create a pull request.

1. **Find your issue number**: Go to [https://github.com/{{full_repo_name}}/issues](https://github.com/{{full_repo_name}}/issues) and note the issue number from Step 1 (it should be about creating a README for project management docs)

2. **Attach the issue to your conversation**: In your Copilot Space, type the following (replace `#` with your actual issue number):

> [!IMPORTANT]
> After typing the issue reference below, press **\<SHIFT\> + \<ENTER\>** to add it to the conversation without sending the message yet.

   ```text
   @{{full_repo_name}}/issues/#
   ```

   (Example: if your issue is #2, type `@{{full_repo_name}}/issues/2`)

3. **Verify the issue is attached**: You should see the issue title and details appear in your conversation

4. **Create the pull request**: Now send this prompt to create the pull request:

   <img width="80%" alt="repository-issue-pr-creation" src="../images/repository-issue-pr-creation-step2.png" />

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

5. **Allow the coding agent**: When prompted, select **Allow** to let the coding agent work on your repository

   <img width="50%" alt="copilot-coding-agent-allow" src="../images/copilot-coding-agent-allow.png" />

6. **Monitor progress**: You should receive a notification that the Copilot coding agent is working on your pull request.

   There are two ways you can check the status of the coding agent working on your pull request

   #### Option 1: Check Pull Requests in your repository

   Go to your repository and click **Pull requests** and select the pull request to see the progress:

      <img width="70%" alt="pull-requests" src="../images/pull-requests.png" />

   #### Option 2: Check Agent Sessions in your Copilot Space on the left side under Agent sessions

   You can track the progress of the Copilot coding agent and view details on the left side under **Agent sessions**. Click on the session to see details about the tasks being performed by the agent.

      <img width="40%" alt="agent-session-1" src="../images/agent-sessions-1.png" />

   You can get to the pull request that the agent is working on by clicking the link in the session details at the bottom where it says **View pull request**.

      <img width="40%" alt="view-pull-request" src="../images/view-pull-request.png" />

7. **Check open pull requests**: We can check pull request status from our **Copilot Space** as well.

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
   >
   > ```prompt
   > check open pull requests
   > ```

   <img width="40%" alt="check-open-prs" src="../images/check-open-prs-2.png" />

   Click the link to the pull request in the Copilot Space to view the PR details and monitor the coding agent's progress.

> [!NOTE]
> The coding agent typically takes 5-15 minutes to complete the work. If you want to track the work that the Copilot coding agent is doing from within the pull request, click **View session** <img width="10%" alt="view-session" src="../images/view-session.png" /> to watch the progress if desired.

8. **Review and merge**: Once the pull request is ready:

   a. **Submit review**: Leave a comment (optional), click **Approve**, then **Submit review**

      <img width="70%" alt="add-review" src="../images/add-review.png" />

      <img width="50%" alt="submit-review" src="../images/submit-review.png" />

   b. **Merge**: Select **Ready for review**, then **Merge pull request** and **Confirm merge**

      <img width="50%" alt="ready-for-review" src="../images/ready-for-review.png" />
      <img width="50%" alt="merge-pull-request" src="../images/merge-pull-request.png" />

<details>
<summary>Having trouble? 🤷</summary>

- **Can't find your issue?** Check the [Issues tab](https://github.com/{{full_repo_name}}/issues) in your repository for the issue you created in Step 1
- **Issue not attaching?** Make sure you're using the exact format `@{{full_repo_name}}/issues/#` where `#` is your issue number
- **Coding agent not working?** Ensure you have the necessary permissions to create pull requests in your repository
- **Pull request creation failed?** The issue must be properly attached before the coding agent can work on it

</details>
