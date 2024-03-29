# mango-website

this branch hosts project page related files

## Setup

Build with MkDocs

```bash
pip install mkdocs
pip install mkdocs-material
```

## Deploy

deploy to github pages

```bash
mkdocs gh-deploy
```

## push and deploy to different repos
say we have `origin` as git remote in the beginning, and we want to use an additional `mgwb` repo to track the development of the website.

First, add the new remote repo:
`git remote add temphosting git@github.com:Oaklight/mgwb.git`

When pull code changes:
```bash
git pull origin # if changes were synced to origin
git pull temphosting # if changes were synced to temphosting
```

When push code changes:
```bash
git push origin
git push temphosting
```

when deploy gh-pages:
```bash
mkdocs gh-deploy -r origin
mkdocs gh-deploy -r temphosting
```

## Structure

```bash
./mango-website/
├── docs
│   ├── assets
│   │   └── images
│   │       ├── mango.png
│   │       └── ...
│   ├── contact.md
│   ├── data.md
│   └── index.md
├── mkdocs.yml
└── README.md
```

- `assets`

    images are stored in `docs/assets/images` folder <br>
    any other assets should be stored in `docs/assets` folder

- `docs` markdown templates

    `docs/index.md` is the home page <br>
    `docs/data.md` is the data detail page <br>
    `docs/contact.md` is the contact page <br>
    any other pages should be added to `docs` folder and linked in `mkdocs.yml`
