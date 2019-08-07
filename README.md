## Using background images in Blender 2.8 

This repository stems from [a discussion I had on Twitter](https://twitter.com/MarkusWerle/status/1158825830824513538), where [@MacSlow](https://twitter.com/MacSlow) offered help. Please check out the PR that fixes [#1](https://github.com/daixtrose/blender-2.8-rendering-with-backgroud-image/issues/1).   

## @MacSlow's Solution 

See #2:

Steps taken to make it work:
- in Render-tab expand 'Film'-property and enable 'Transparent'
- go to Compositing-layout, enable 'Use Nodes'
- via Shift-a shortcut create nodes: 'Input/Render Layers', 'Input/Image', 'Distort/Scale', 'Color/Z Combine', 'Output/Composite' and 'Output/Viewer'
- (examine node setup from this repo's project file)
- hit F12 (the compositing will not start before render-step is completed)
