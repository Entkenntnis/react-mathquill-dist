# react-mathquill-dist

### Why?
Unfortunately, [mathquill](https://github.com/mathquill/mathquill) has no recent npm releases. So we need to build it ourselves, inlcuding [react-mathquill](https://github.com/viktorstrate/react-mathquill).

### How?
Follow these steps to reproduce this repository:
1. Clone mathquill
2. Run `npm install` and `make` in the root directory of mathquill. Notice: Mathquill is using make, sh, etc. to build, so a linux environment is necessary.
3. Clone react-mathquill
4. Run `npm install`
5. Override the content of `react-mathquill\node_modules\mathquill\build` with the content of `mathquill\build`
6. Build react-mathquill with `npm build`
7. Keep the `dist` folder and all files of the root directory.

### Usage
To use this repository, edit your package.json and add `"react-mathquill": "git+https://github.com/Entkenntnis/react-mathquill-dist.git"`