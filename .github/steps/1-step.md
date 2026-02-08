## Step 1: Create and prime your Copilot Space

In this step you will establish a Copilot Space and give it the minimum context it needs to act as a project management knowledge hub for OctoAcme.

### How does using Spaces affect my usage?

Questions you submit in a space count as Copilot Chat requests.

- If you're a Copilot Free user, this usage counts toward your monthly chat limit.
- If you use Spaces with a premium model, this usage counts toward your premium usage quota. Every question you submit to a premium model counts as one premium request, multiplied by the model's multiplier. For information about the multipliers applied to each model, see [Requests in GitHub Copilot](https://docs.github.com/en/copilot/managing-copilot/understanding-and-managing-copilot-usage/understanding-and-managing-requests-in-copilot#model-multipliers).

- [Use Copilot Spaces](https://docs.github.com/en/copilot/how-tos/provide-context/use-copilot-spaces/)

### 📖 Theory: Using Copilot Spaces as a Knowledge Hub

GitHub Copilot Spaces enables teams to centralize and democratize organizational knowledge by providing a collaborative environment for storing, searching, and refining process documentation. By connecting your repository as a source, Copilot Spaces can index your documentation and issue templates, making them easily accessible and actionable for all team members. This approach reduces single-person dependency risk, accelerates onboarding, and ensures that project management processes are consistent and repeatable.

To get started, you need access to Copilot Spaces and a GitHub Copilot plan with premium request units. Each prompt in a Space counts toward your usage quota, so be mindful of your plan's limits. For more details, see [GitHub Copilot plans](https://docs.github.com/en/copilot/get-started/plans#comparing-copilot-plans) and [Copilot Requests](https://docs.github.com/en/copilot/concepts/billing/copilot-requests).

> [!NOTE]
> Questions you submit in a Copilot Space count as Copilot Chat requests. Premium models multiply usage. See [Requests in GitHub Copilot](https://docs.github.com/en/copilot/managing-copilot/understanding-and-managing-copilot-usage/understanding-and-managing-requests-in-copilot#model-multipliers) for details.

### ⌨️ Activity: Create your OctoAcme Project Management Hub Copilot Space

1. Navigate to GitHub Copilot Spaces https://github.com/copilot/spaces (ensure you have access to this feature)
1. Click **Create Space** button
1. Name your Space:

   > ```text
   > OctoAcme Project Management Hub
   > ```

1. Click **Save**

   <img width="50%" height="50%" alt="Copilot Space Create Space" src="https://github.com/user-attachments/assets/0dcc4d78-1ee0-43cf-85c8-c1d0137aceb0" />

Add a description:

> ```text
> Centralizing and democratizing project management knowledge for the OctoAcme organization
> ```

   <img width="50%" height="50%" alt="Copilot Spaces description" src="https://github.com/user-attachments/assets/5826b4bc-a40b-4705-b36a-66b234c2c07d" />

### ⌨️ Activity: Add instructions to your Copilot Space

- In your newly created Copilot Space, look for the **Instructions** button
- Add the following instructions to provide context about the repository and its purpose

  <img width="50%" height="50%" alt="Copilot Spaces Instructions" src="https://github.com/user-attachments/assets/547cdbf9-9238-42af-a06b-7bb168207ec2" />
  <img width="50%" height="50%" alt="Copilot Spaces Instructions detail" src="https://github.com/user-attachments/assets/628b8534-5f14-48ba-89dc-16eec79617ea" />

- Click **Save**

  > ```markdown
  > ## Program process documents
  >
  > - Stored in `docs/`
  >
  > ### Purpose of this Copilot Space
  >
  > - Centralize scattered project management knowledge in Copilot Spaces
  > - Convert tacit team insights into searchable, versioned artifacts
  > - Give all team members equal access to processes, decisions, and rationale
  > - Connect a repository as a structured knowledge source
  > - Extract, refine, and standardize workflows collaboratively
  > - Feed validated improvements back into living documentation
  > - Accelerate onboarding and reduce single-person dependency risk
  > - Enable consistent, repeatable project execution
  >
  > ## Issue templates for program process documents
  >
  > - Stored in `.github/ISSUE_TEMPLATE/`
  > ```

### ⌨️ Activity: Add your cloned repository as a source repository to your Copilot Space

1. In your newly created Copilot Space, look for **Add sources** button
1. Add this exercise repository as a source:
   - Copy and paste your GitHub repository for this exercise called out below.
   - You can also type the name in the search and it will come up as well or copy/paste the name below.

     > ```text
     > {{full_repo_name}}
     > ```

   - This gives Copilot access to the project management documentation and processes in the repository

1. Select the `docs` and the `.github/ISSUE_TEMPLATE` folders
1. Verify the repository appears in your sources list

  <img width="30%" height="30%" alt="Add sources" src="https://github.com/user-attachments/assets/05268c3f-5270-4e60-bc87-69fc27b1df72" />
  <img width="30%" height="30%" alt="Add sources repository" src="https://github.com/user-attachments/assets/83725fcc-eb0d-4478-ba88-8de0cd8a6732" />
  <img width="30%" height="30%" alt="Add sources repository files" src="https://github.com/user-attachments/assets/f3e9c65a-1446-4f1f-a84f-10f893d0e22e" />

### ⌨️ Activity: Create an issue in the repository for a README for OctoAcme Project Management Docs

- Open your Copilot Space you created above. https://github.com/copilot/spaces
- In the conversation interface prompt the following:

  > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=social&logo=github%20copilot)
  >
  > ```prompt
  > Create an issue in the repository {{full_repo_name}} for a README for OctoAcme Project Management Docs
  > that has links to all the docs in the docs folder.
  > - The README should also contain a brief summary of the project management processes used by OctoAcme.
  > - Make sure README, project management processes summary, and links are in the title of the issue.
  > - Use the "Add Content to Project Management Process Docs" template.
  >  - Which process document do you want to update? "<new document>"
  >  - Fill in the other fields
  > ```

You can then add this issue to your repository by clicking the **Create** button.

<details>
<summary> 📷 Show screenshot of the issue draft</summary>

<img width="50%" height="50%" alt="README issue drafted" src="https://github.com/user-attachments/assets/fd324605-a02b-4d4a-a87f-06db9339bb44" />

</details>
You can copy or open the link in a new tab to see the newly created issue

<details>
<summary> 📷 Show screenshot of the created issue</summary>

<img width="50%" height="50%" alt="README issue created" src="https://github.com/user-attachments/assets/c4be58b8-edbf-463a-be49-8ad184d59617" />

</details>

<details>
<summary>Having trouble? 🤷</summary>

- Make sure you have access to GitHub Copilot Spaces (currently in beta/limited access)
- The repository should be publicly accessible for Copilot to index it
- If you can't access Copilot Spaces, you can continue by manually exploring the repository structure and documentation
- Repository indexing can take seconds to minutes depending on size

</details>
