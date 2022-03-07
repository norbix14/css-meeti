# Meeti

## Screenshots

![Header](screenshots/header.png "Header")
![Search](screenshots/search.png "Search")
![Events](screenshots/events.png "Events")
![Categories](screenshots/categories_001.png "Categories")
![Categories](screenshots/categories_002.png "Categories")
![Groups](screenshots/groups.png "Groups")
![Footer](screenshots/footer.png "Footer")
![Meeti](screenshots/meeti.png "Meeti")

## Installation

### clone repo

* **gh CLI**

```bash
gh repo clone norbix14/css-meeti meeti
```

* **git**

```bash
git clone https://github.com/norbix14/css-meeti.git meeti
```

### folder

```bash
cd meeti/
```

### install dependencies

```bash
npm i
```

## before run the app

### **gulp** tasks

* optimize *png or jpg* images (from **./src/images_raw/** to **./src/img/**)

```bash
gulp optimizeImages
```

* build **webp** images (transform **all** images into *.webp*)

```bash
gulp buildImagesWebp
```

* build **avif** images (transform **all** images into *.avif*)

```bash
gulp buildImagesAvif
```

* manually transform *scss* into *css*

```bash
gulp buildCss
```

* watch changes in *scss* files (same as *gulp* command below)

```bash
gulp dev
```

* transform *scss* into *css* (default task) and watch for changes

```bash
gulp
```

### copy files into **dist** (Linux Ubuntu)

* copy all files recursively except:
  * *images_raw* folder which is optimized by **gulp** in the *img* folder
  * *scss* folder wich is transformed by **gulp** in the *css* folder

```bash
cp -r src/!(images_raw|scss) dist/
```

## run the app

* using the current folder

  * double click on **src/index.html** or open it with **Live Server**

* using the **dist** folder

  * double click on **dist/index.html** or open it with **Live Server**
