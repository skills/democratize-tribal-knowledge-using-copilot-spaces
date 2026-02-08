## Step 3: Create an issue and pull request to improve project management processes

In this step, you will practice iterative process improvement by:

1. Creating a GitHub issue using an issue template to document needed improvements to personas/roles in project management processes
2. Using GitHub Copilot's coding agent to automatically create a pull request that implements these improvements

This demonstrates a complete improvement workflow: identify gaps (issue) → implement solutions (pull request) → maintain traceability (linked in Copilot Space).

### 📖 Theory: Iterative Process Improvement

Effective process evolution follows a lightweight cycle:

- Review current documentation and execution reality
- Identify gaps, ambiguities, or missing personas/roles
- Record the need as a structured issue (problem statement + rationale)
- Design and implement improvements (docs, templates, checklists) in a PR
- Communicate changes via clear descriptions and linked artifacts
- Measure adoption and revisit as new insights emerge

> [!IMPORTANT]
> Use the **GPT-4.1** model for all conversations with Copilot Spaces.

### ⌨️ Activity: Attach an issue template and create an issue for process improvements

_Use the following prompt in a new Copilot Space conversation:_

- Select your repository

  > ```text
  > {{full_repo_name}}
  > ```

- Select the issue template to this new Copilot Space conversation. </br>
  `.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml`

     <img width="30%" height="30%" alt="Attach" src="https://github.com/user-attachments/assets/2a447ff9-76d7-462f-9292-4663c8dc0fc9" />
     <img width="30%" height="30%" alt="Attach files" src="https://github.com/user-attachments/assets/6ac6e33d-b333-424f-b431-e3feb7022b84" />

     <img width="30%" height="30%" alt="Attach issue template conversation" src="https://github.com/user-attachments/assets/5fc71905-ede6-45cb-bcfa-93d2797160b2" />

  > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
  >
  > ```prompt
  > Use the attached issue template
  > - Identify potential new personas/roles that could be added to the project management processes documentation
  >   to enhance clarity and accountability.
  > - Create an issue titled "Adding more personas and roles to the project management processes"
  >    that outlines the need to expand the defined roles and responsibilities in the project management documentation.
  > - Make sure the new roles/personas have descriptions of their responsibilities and how they interact with existing roles.
  > - The issue should detail why this is important, potential personas to add, and how it will improve project outcomes.
  > - add to the process document `docs/octoacme-roles-and-personas.md`
  > ```

    <img width="50%" height="50%" alt="personas/roles issue draft" src="https://github.com/user-attachments/assets/cd02e396-2505-450a-aca3-8e1642d6306a" />

  <img width="50%" height="50%" alt="personas/roles issue created" src="https://github.com/user-attachments/assets/7f30e13b-7efd-45a0-939a-e7095ff0637c" />


### ⌨️ Activity: Attach an issue and create a Pull Request

_Use the following prompt in the current Copilot Space conversation:_

In the same Copilot Space conversation do the following:

1. In this activity we will attach the issue you created in the previous activity
2. This will assign the issue to the coding agent to create a pull request with an update to our personas/roles document in the `docs/` folder
3. Copy and paste the url for the issue that we created in the previous activity. </br>

> [!NOTE]
>
> - Make sure the issue below matches the issue you want to attach
> - Hit **\<SHIFT\> + \<ENTER\>** so you don't start Copilot working on the conversation

Check issues list: [https://github.com/{{full_repo_name}}/issues](https://github.com/{{full_repo_name}}/issues) </br>

> ```text
> @{{full_repo_name}}/issues/4
> ```

   <img width="40%" height="40%" alt="repository issue and pull request creation" src="https://github.com/user-attachments/assets/cf4f0c32-76cb-429d-b607-f65f444b07d5" />

> ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
>
> ```prompt
> - Using the github-coding-agent tool create a pull request that implements process improvements
>   based on the analysis we did earlier.
> - The improvements should address gaps or inefficiencies identified in the project management documentation.
> - The pull request should include updates to existing docs or new templates/checklists as needed.
> - All documents should be in the `docs/` folder
> - Add this pull request to the attached issue.
> - Add {{login}} as a reviewer for this pull request
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

   <img width="40%" height="40%" alt="mission control" src="https://github.com/user-attachments/assets/66693282-e5f6-45d6-8ca8-968e73826738" />

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

- Focus on the most impactful improvements identified in your analysis
- Consider adding templates, checklists, or clarifying existing processes
- Common improvements include: role clarification, communication protocols, decision-making frameworks
- Even small improvements like adding examples or clarifying steps can be valuable

</details>
