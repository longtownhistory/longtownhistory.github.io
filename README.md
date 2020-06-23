# longtownhistory.github.io
## Remembering Freedom Longtown History Harvest

The Greenville Settlement was one of the earliest and most prosperous rural Black communities in the states of Indiana and Ohio. Much of what once existed of the settlement is no longer there. The Clemens farmstead, a declining ULI building, and three cemeteries (one neglected in the middle of a white-owned farm) are what remain of the settlement in its physical form.

The settlement has been preserved in the memories of its descendants. The descendants’ grassroots preservation work takes shape in a variety of ways: archiving historical documents and artifacts, attaining historical markers, restoring old buildings, registering buildings on the National Register of Historic Places and as an Underground Railroad site by the National Park Service, and maintaining a very active descendant-run Facebook page.

This History Harvest, which took place in September 2019, is an exciting addition to those preservation practices.

Communities hoping to build their own history harvest using this repository can copy it and then use the elements that best suit their community needs:

### The initial setup

Have a look at the video walkthrough version of this at: https://youtu.be/LM-w5wZvtJo

1. Registering a GitHub user is the first step. Choose a username that represents your project well, because that's what the URL will be if you're using the free version of Github Pages
2. Create a repository called "*username*.github.io"
3. Copy the contents of this repository into it.
4. Enable Github Pages in settings
5. Make changes to the file called "_config.yml" in the main repository directory

### Putting the basics together

The best way to create a community history harvest is to look through the files in this repository and see what they do in the public-facing web site.

Compare the files at https://github.com/longtownhistory/longtownhistory.github.io/ with the pages that display at https://longtownhistory.github.io/

- Descendants (found in the "descendants" folder) are the members of the community whose memories and heirlooms are preserved. Some descendants may have memories, some may have items, some may have both. Each descendant should have a "folder" name so that their items and memories can be easily tied together. The "title" field should contain their full name.
- Items (found in the ["items"](https://github.com/longtownhistory/longtownhistory.github.io/tree/master/_items) folder) are the individual heirlooms preserved by descendants. The YAML front matter or metadata has information about the item. This is always at the beginning of each individual item file, and the information here helps organize and present items as part of a descendant collection and as part of the multi-family collection. Each item should have a unique id (e.g. 15h or smithville1) and the folder name that helps connect that item to the descendant who preserved it.
- Memories (found in the "oralhistories" folder) are individual memories preserved by descendants. As with items, the lines at the beginning of each oral history file help connect those memories to the descendants and their collections. For interviewees who don't have associated collections of physical items, we add their full name here.

These basics are displayed by using the ["collections" feature of Jekyll](https://jekyllrb.com/docs/step-by-step/09-collections/). Collections are described in the main "_config.yml" file.

Once your community has made decisions about which of these features it needs, find the items, descendants, and memories examples that best fit your community's needs. Keep those files and delete the rest. Copy and paste the content from these files and use them as templates to preserve your community's history.

### Editing items and adding images

Have a look at the video walkthrough version of this at: https://youtu.be/aqMoGK50vt0

Items are the easiest place to start. Add a new item by copying and pasting the elements of an existing item into a new item by using the "Create File" button when you're inside the \_items folder.

Item images are in the ["/assets/collections"](https://github.com/longtownhistory/longtownhistory.github.io/tree/master/assets/collections) folder, nested in a folder named for each descendant. Items can have many photos associated with them. Simply name the photo with the item's unique ID and then an underscore and a number (e.g. 15g_1.jpg, 15_2.jpg).

Each item should also have a smaller thumbnail (cropped to 768 pixels square on both sides) and named after the item id with a "\_th" added (e.g. 15h_th.jpg)

### Customizing colors and fonts.

Most of the customization can be done in the file at ["/assets/css/main.scss"](https://github.com/longtownhistory/longtownhistory.github.io/blob/master/assets/css/main.scss).

#### Color choices

Web-based platforms use something called "hex color": a 6-digit color "ID" with 2 digits each for red, green and blue. For instance, bright red is #cc0000. Choose colors here: [https://htmlcolorcodes.com/color-picker/](https://htmlcolorcodes.com/color-picker/). Search and replace our colors with yours:

- light background: fbf2e3
- nav-bar text: faf5e8
- headers: 592a07
- links: 733d15
- visited links: 9f6233

#### Font choices

Web-based platforms also need to load special fonts each time a new page is loaded. [Google Fonts](fonts.google.com) provides fonts free of charge and has an easy to use "embed code" creator. If your community chooses to change fonts, the new font will need to be embedded in the "/\_layouts/default.html" file on line 20 and changed in the main.scss file on lines 8, 37, 41.
