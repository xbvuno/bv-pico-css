
# bv-pico-css
A custom version of picocss for my projects
[Original framework](https://picocss.com/)  (Built at v2.0.6)
## How to build (on Windows):
### Explaination
- Legend: 
	 - '*':  **Optional**
	 - '**' : Optional but the rest of the commands **rely** on that
	 - If no asterisk, it means **required**

- Download [Sass](https://sass-lang.com/)  
	- `\> npm install -g sass`**
	- Close and reopen the terminal
- Don't do your things in random folders, make a new one
	-  `mkdir build-folder`**
	- `cd build-folder`**
- Clone the [pico](https://github.com/picocss/pico) repo, you need the `scss` folder
	- `\build-folder> git clone https://github.com/picocss/pico.git`,
	- `\build-folder> move pico\scss .\` **
	- `\build-folder> rm -Force pico` *
- Clone this repo and put the files in the `scss` folder
	- `\build-folder> git clone https://github.com/xbvuno/bv-pico-css.git`
	- `\build-folder> move bv-pico-css\* scss`
- Use Sass to compile in css and update it as you edit with `--watch`
	- `\build-folder> sass ./scss/main.scss:dist/bvuno-pico.css --watch`
- Edit the style as you want
	- Follow [this guide](https://picocss.com/docs/sass)
- You can find the output file in `/dist/` as `bvuno-pico.css`
- If you just need the `.css` file, take it and delete all the rest
  	- `\build-folder> cd .. `**
  	- `\> move build-folder\dist\bvuno-pico.css .\` **
 

```
npm install -g sass
```
```
mkdir build-folder 
cd build-folder
git clone https://github.com/picocss/pico.git
move pico\scss .\
rm -Force -Recurse pico
git clone https://github.com/xbvuno/bv-pico-css.git
move bv-pico-css\* scss
sass ./scss/main.scss:dist/bvuno-pico.css
cd ..
move build-folder\dist\bvuno-pico.css .\
rm -Force -Recurse build-folder

```
