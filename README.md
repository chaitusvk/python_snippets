# python_snippets
python snippets for easy refer back

# Load images Names Ending with *.png
### Path to the data directory
```data_dir = Path("./captcha_images_v2/")```
### Get list of all the images
```images = sorted(list(map(str, list(data_dir.glob("*.png")))))
labels = [img.split(os.path.sep)[-1].split(".png")[0] for img in images]```
