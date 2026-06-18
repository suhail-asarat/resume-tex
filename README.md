# LaTeX Resume Template

A clean, highly customizable, and ATS-friendly LaTeX Curriculum Vitae (Resume) template with support for a profile picture and semantic data commands.

## How to Create Your Own Resume

To build your own Resume, you will primarily be editing the `resume.tex` file. 

1. Copy or download `resume.tex`, and `resume.sty`.
2. Open `resume.tex` in your preferred LaTeX editor.
3. Update the `\resumeHeader`, and subsequent sections with your personal information, work experience, education, etc.
4. Compile the document to generate your `resume.pdf`.

Below are three popular ways to edit and compile your Resume.

---

### Option 1: Using Overleaf (Free Tier)

Overleaf is a great web-based LaTeX editor. You can use it for free without linking a GitHub account by uploading your files manually.

1. Create an account or log in at Overleaf.
2. Click on **New Project** and select **Blank Project**. Give it a name.
3. In the left-hand file tree, delete the default `main.tex` file.
4. Click the **Upload** icon (top left of the file tree) and upload the following files from your computer:
   - `resume.tex`
   - `resume.sty`
5. Change the main document setting so Overleaf knows which file to compile. Click the **Menu** button (top left), look for the **Main document** dropdown, and select `resume.tex`. *(Alternatively, you can just rename `resume.tex` to `main.tex`)*.
6. Click **Recompile** to generate and view your PDF!

---

### Option 2: Using Dev Containers (VS Code)

If you prefer an isolated local environment using Docker to avoid installing LaTeX directly onto your host OS, you can use Dev Containers.

1. Ensure you have Docker installed and running.
2. Install Visual Studio Code and the **Dev Containers** extension (`ms-vscode-remote.remote-containers`).
3. Open this folder in VS Code.
4. If prompted, click **Reopen in Container** (or press `F1` and run `Dev Containers: Reopen in Container`). This will build a container with LaTeX pre-installed (assuming a `.devcontainer` configuration is present in your project).
5. Once the container is built and running, open `resume.tex` and compile using the integrated LaTeX tools provided by the container.

---

### Option 3: Local Setup with TeX Live and VS Code

For a fully local, native setup, you can install a LaTeX distribution directly on your machine.

1. Install **TeX Live** (or MacTeX for macOS, MiKTeX for Windows).
2. Install Visual Studio Code.
3. Install the **LaTeX Workshop** extension by James Yu (`james-yu.latex-workshop`) from the VS Code extension marketplace.
4. Open the folder containing your Resume files in VS Code.
5. Open `resume.tex`.
6. Press `Ctrl+Alt+B` (or `Cmd+Option+B` on Mac), or click the green "Play" (Build) icon in the top right corner of the editor to compile the document. The extension will automatically use your local TeX Live installation to generate the PDF.