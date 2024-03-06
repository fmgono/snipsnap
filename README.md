<img src="https://raw.githubusercontent.com/fmgono/snapsnip/master/public/logo.png" width="80px" height="80px"/>

# SnapSnip
> A Fast, tiny, in-browser, IndexedDB powered editor and Snippet manager

Built with [Vue.js](https://vuejs.org), [Dexie](https://dexie.org) and [Monaco Editor](https://microsoft.github.io/monaco-editor/) . SnapSnip provides a clean and VSCode like familiar interface to save notes, tasks and code snippets directly in the browser. 
> All the data is stored within your browser tab (IndexedDB). There is no cloud backup available so far but you can still create backups and restore/share your contents with others.

## Features
- Syntax Highlighting 
- Easy to use Document files (.doc) using ProseMirror Editor
- MultiWindow Editing (Drag and drop files to the editor area to switch to multi editor)
- Quick Create (Ctrl+N)
- Shortcuts for most of the actions (Create, Rename, Delete, etc..)
- Ability Import and Export your data

![Screenshot_2021-04-13 Snipp in - In browser notes and code snippets](https://user-images.githubusercontent.com/53584487/115232100-fcb42300-a133-11eb-803f-45efa41fc719.png)
![Screenshot_2021-04-12 Snipp in - In browser notes and code snippets](https://user-images.githubusercontent.com/53584487/115232151-05a4f480-a134-11eb-9033-cf696f38d1f2.png)


## Project setup
```
git clone https://github.com/fmgono/snapsnip snippin
cd snippin
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```
### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).



## Docker Setup

You can use SnapSnip from docker, you can build your own image using 

```
docker build -t snipp/SnapSnip .
```

To depoly an SnapSnip instance using docker container you can run the following: 


```
docker run -it -p 80:80 snipp/SnapSnip .
```

You can change the host binding port from `80` to other ports. 

Now to access the instance you can go to browser and write `http://localhost` or your `ip:port` if you deploy on a vps (public instance) and changed the host binding port.


