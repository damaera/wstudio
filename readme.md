## How to add posts
you can add new post for new project

in folder `_posts` create file with following format `YYYY-MM-DD-your-name.markdown`

edit the content, and data
first, always begin with triple dash, and end with triple dash

| key  | value  |
| --- | --- |
| layout  | post [dont change this!] |
| title | Your Title |
| permalink | where your link will appear `work/bla-bla-bla` |
| project_type | yout project type |
| client | yout client |
| location | yout project place |
| area | yout project area |
| building_area | yout project build area |
| project_year | yout project year |
| cover | default cover, image number X |
| image-folder | name of your folder images |
| images-count | count of your images, excluding floor plan |
| denah-count | count of your denah |

## Upload images

to upload images.

in folder `images`, create new folder with a name, for example `klg-cemara`. then, name the building images with `X.jpg` with x is number. must in order from 1. for example `1.jpg`, `2.jpg`, `3.jpg`. then the floor plan, naming format with `dX.jpg`. for example `d1.jpg` then `d2.jpg`.

consider you upload 5 images, 2 denahs, and want 2.jpg to be cover in folder `klg-cemara`
then in your `post` edit the data.
```
cover : 2
image-folder : klg-cemara
images-count : 5
denah-count : 2
```

that's it!