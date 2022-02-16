## Dancing with AI Curriculum 

[Live Preview](https://dancingwithai.media.mit.edu)

## Getting Started

1. Make sure you have Ruby installed
2. `bundle install`
3. `bundle exec jekyll serve`
4. Visit http://localhost:4000 

# Deployment

See Jekyll's [Deployment Methods](https://jekyllrb.com/docs/deployment-methods/) website for more info!

If using GitHub, make sure GitHub Pages is enabled for your repo. It might take some time for the site to build and deploy.

## Customize

Things you can customise in `_data/settings.yml` (no HTML/CSS):

- Theme Settings
- Curriculum content

## Acknowledgements + Licenses

- Theme + Jekyll from Themefisher (https://themefisher.com/) (https://github.com/themefisher/kross-jekyll-portfolio-template/blob/master/LICENSE.txt)
- Pirate Project background: <a href="https://www.freepik.com/free-photos-vectors/background">Background vector created by freepik - www.freepik.com</a>
- Recycling images <a href="https://www.freepik.com/free-photos-vectors/food">Food vector created by photoroyalty - www.freepik.com</a>
- Snake game technique from "Snake red" by bigbang2 https://scratch.mit.edu/projects/11203511/

## Contributing 

### Adding scratch projects

The [generated site](https://dancingwithai.media.mit.edu) (automatically deployed using [github pages](https://pages.github.com/)) is used to host examples of Scratch projects that leverage PRG's 'poseblocks'. This allows for an easy way to share poseblock-based experiences and let users *remix* them without having to download them onto their computer. 

When adding a project, you can choose whether or not you'd like to have the project featured in the [site's](https://dancingwithai.media.mit.edu) 'project gallery' (check out the ***"Try Some Projects!"*** section). If not, meaning you'd just like to have the project accessible via link, you only need to follow [Step 1](#step-1) below. If you'd like to both have the project accessible via link, as well as featured in the site's project gallery, follow both [Step 1](#step-1) and [Step 2](#step-2) below. 

#### Step 1:
##### Add your files

Conveniently, you can add project files without ever having to clone this repositiory. Simply do the following:

1. Navigate to the repo's [projects upload page](https://github.com/dancingwithai/dancingwithai.github.io/upload/master/projects)
3. The above link will bring you to a new page where you can:
    - Choose the files you'd like to upload
      - **NOTE:** You should upload a `.gif` demonstrating your project in addition to the `.sb3` project file. If you won't be adding your project to the project's gallery in [Step 2](#step-2), it's not necessarily required, but you'll just need to remember to add a `.gif` later if you'd like add the project to the gallery. So might as well do it now! 
    - Commit the changes directly to the `master` branch (please ensure the commit message and description are clear), which will automatically trigger the site to re-deploy.
4. Once the site is succesffully deployed, your files will be located at the following link: 
> https://dancingwithai.media.mit.edu/projects/$THE_NAME_OF_YOUR_PROJECT.sb3 

(please subsitute out $THE_NAME_OF_YOUR_PROJECT with the appropriate name of your project)
    - You can look at the progress of the deployment in the [Actions panel](https://github.com/dancingwithai/dancingwithai.github.io/actions)

#### Step 2:
##### Associate your files with the site's data 
  
Conviently, you can (also) add your newly-added project files as an entry to the 'projects gallery' without cloning the repo. Simply do the following:
  
1. Navigate to an editable version of the site's [data configuration file](https://github.com/dancingwithai/dancingwithai.github.io/edit/master/_data/settings.yml)
  - **NOTE:** The above link will take you directly to the editable version of the [data configuration file](https://github.com/dancingwithai/dancingwithai.github.io/blob/master/_data/settings.yml), as if you navigated to the file and clicked the 🖊️ 'Edit this page' button.
2. Add an entry to the `all-projects` list that begins on [line 273](https://github.com/dancingwithai/dancingwithai.github.io/blob/master/_data/settings.yml#L273)
  - Your entry should look like the following: 
  ```yaml
  - image: "$your_projects_gif.gif"
    url: "$your_projects_name.sb3"
  ```
3. Commit the changes directly to the `master` branch (please ensure the commit message and description are clear), which will automatically trigger the site to re-deploy.
    - You can look at the progress of the deployment in the [Actions panel](https://github.com/dancingwithai/dancingwithai.github.io/actions)
