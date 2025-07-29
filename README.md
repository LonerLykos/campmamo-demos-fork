# Camp Mamo Demos

Welcome to the **Camp Mamo Demos** repository!  
This repo is the single place where participants in **Camp Mamo**—Celestia's hackathon preparation program—can find, pull, and explore every example project used throughout the course.

---

## 📚 What is this repo?
Camp Mamo spans many topics and hands-on sessions. To keep things organised we host each demo or reference implementation in its **own standalone Git repository**.  
This repo is therefore an **anchor / index**: every top-level folder here points to another repository that holds the actual demo code.

We keep these external repos as **Git submodules** so that you can:
1. fetch everything with a single clone command;
2. stay in sync with upstream fixes and improvements;
3. avoid inflating the size of this meta-repo.

If the term *submodule* is new to you—don't worry, the commands you need are listed below.

---

## 🚀 Quick start
```bash
# Clone *and* pull all submodules in one go
$ git clone --recurse-submodules git@github.com:celestiaorg/campmamo-demos.git

# If you already cloned without the flag, run:
$ git submodule update --init --recursive
```
Each sub-folder now contains a fully-functional project ready for you to open, build, and hack on.

---

## 📦 Large files (Git LFS)
Some demos (such as `dojo-demo`) track game assets or other binaries using **Git LFS**. If you don't have it installed yet, run:

```bash
# macOS (Homebrew)
brew install git-lfs

# Linux (apt example)
sudo apt-get install git-lfs

# One-time global setup
git lfs install
```
After cloning this repo, Git LFS files will be pulled automatically the first time you access a directory that needs them. You can also fetch everything explicitly with:

```bash
git lfs pull --all
```

---

## 🗂️ Repository layout
```
campmamo-demos/
├── dojo-demo/            # ↳ https://github.com/gbarros/dojo-demo (submodule)
├── chopin-demo/          # placeholder – upcoming demo
├── initia-demo/          # placeholder – upcoming demo
├── livy-demo/            # placeholder – upcoming demo
├── rollkit-demo/         # placeholder – upcoming demo
└── LICENSE               # licence information for this index repo
```
> The exact list will grow as the course progresses. Check back often or run `git pull --recurse-submodules` to stay up-to-date.

---

## 🎨 Brand assets

Need graphics for your Camp Mamo project or social media posts? We've got you covered!

### Brand Kit
Access our complete brand kit with logos, colors, and design guidelines:  
📁 **[Camp Mamo Brand Kit](https://drive.google.com/drive/folders/1kZuEknsnXz_XvXQUVBQkX4i8DD3WGFeC)**

### Create Your Own Graphics
Use our Figma templates to create custom graphics for your projects:  
🎨 **[Camp Mamo Shareables - Figma](https://www.figma.com/design/AodtIu10eBxHEKMIXe7UMI/Camp-Mamo-shareables?node-id=0-1&t=yMnRo3YdvQTYiqdI-1)**

**How to use the Figma templates:**
1. **Sign in to Figma** with your account
2. **Copy the graphic** you want to use from our template
3. **Paste into your own Figma project** and edit it to your liking
4. **Select your artboard** (e.g., "Landscape X 16:9") and click **"Export"** in the bottom right
5. **Share your graphic** on Twitter and tag us!

---

## 🤝 Contributing & adding new demos
1. Fork this repo and create a new branch.
2. Add the external demo as a submodule:
   ```bash
   git submodule add <demo-repo-git-url> <folder-name>
   ```
3. Commit and push your changes, then open a pull request.  
   Remember to include a short description of the demo and a link to its documentation in the PR body.

Please keep new demos small and focused—participants should be able to clone everything quickly.

---

## 📄 Licence
The content of **this** repo is licensed under the **Apache License 2.0** (see `LICENSE`).  
Each submodule keeps its own licence; make sure you comply with it when re-using code.

---

## 🙋 Need help?
If you hit any issues, open an [issue](https://github.com/celestiaorg/campmamo-demos/issues) or post in the Camp Mamo Discord. We're happy to help!

Happy hacking! 🚀