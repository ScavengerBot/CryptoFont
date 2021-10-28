# Cryptocurrency Icon Font
A cryptocurrency font with over 400+ icons and actively being added to. <br>
Check out the [demo](https://codepen.io/oneezy/pen/YzWLxPO).


## Usage
Install locally
```
npm install @scavengerbot/cryptofont
```
Or use with CDN
```
https://cdn.jsdelivr.net/npm/@scavengerbot/cryptofont/style.css
https://cdn.jsdelivr.net/npm/@scavengerbot/cryptofont/style.min.css
```
## Designing Icons
1. Find the original SVG icon and add it to the `icons/original` folder
2. Open the `icons/starter.svg` file in **Adobe Illustrator**
3. Scale the original icon down to the correct pixel dimensions `(32x32)`
4. Icon fonts can't be multicolored so choose the color best suited for the icon and apply it to the circle (ellipsis)
5. Center the icon on top of the ellipsis (`Horizontal Align Center` and `Vertical Align Center`) the icons on 6. Use the **Pathfinder** tool to cut out the shape from the circle (`Minus Front`)
7. Select all the paths you want to merge and exclude any internal paths you do not
8. Open your **Pathfinder** and click `Unite` to merge the objects
9. Go to top menu and click `Object` tab, in drop down choose `compound path` and click `make` or you press `ctrl+8`
10. When finished `Save As` to the `icons/color` folder and name the icon correctly (this name will be the name used in the css class)

## Contributing Icons
1. Fork the repo
2. Clone the repo
3. Navigate to the project on your local machine
4. Pull the latest changes
5. Create a new feature branch
6. Add original svg icons (multicolor) to the `icons/original` folder
7. Add new svg icons (1 color) to the `icons/color` folder
8. Go to [icomoon](https://icomoon.io/app) and import the `selection.json` file and click **YES** to settings
9. Drag and Drop new icons from `icons/color` folder into icomoon and be sure they are selected
10. Drag and Drop selected icons to bottom
11. Click "Generate Font" at bottom right and then "Download"
12. Replace everything in the local folder with the newly downloaded folder
13. Update the `package.json` version number i.e. *(1.3.0 to 1.4.0)*
14. Commit your changes and list which icons were added
15. Push your changes to your fork
16. Create the Pull Request

## For project maintainers
1. When new PR's come in, test everything before merging
2. Make sure the `package.json` version is bumped up
3. Merge the PR and remove the feature branch
4. Publish package to NPM `npm publish`
5. Update [codepen demo](https://codepen.io/oneezy/pen/YzWLxPO)
6. Purge npm cryptofont stylesheet to receive [new version](https://cdn.jsdelivr.net/npm/@scavengerbot/cryptofont@latest/style.min.css)
## Special Thanks 👏

To those involved at SPOTHQ (https://github.com/spothq/cryptocurrency-icons) for the start.


## Used By
- [ScavengerBot](https://scavengerbot.io)