## Model Annotation for Cell Tracking Challenge dataset

![](https://github.com/DevoLearn/Model-Annotation/blob/main/Media/E_RsexVXMAQESDN.jpg)

In conjunction with the [OpenWorm Foundation](https://openworm.org/) and [Orthogonal Research and Education Lab](https://orthogonal-research.weebly.com/)   

# C. elegans Image Annotation for Hacktoberfest

Hello, contributors! 🎃 Welcome to our Hacktoberfest project. We're aiming to annotate a dataset of C. elegans images to fine-tune the Detection 2 model and SAM segmentation for an upcoming GSoC project. Your contribution will play a pivotal role in advancing research in this area.

## 📂 Dataset Structure

- `images/`: Contains the C. elegans images.
- `segmentation_maps/`: Contains the segmentation maps for the images.
- `data.csv`: A CSV file listing the image file names.

## 🎯 Task

We need bounding boxes around each C. elegans cell in the images.
dataset [link](https://drive.google.com/file/d/1ZMFMsd7d6R-PFju3QpZlb26zbaNcrFf9/view?usp=share_link),
csv_file [link](https://drive.google.com/file/d/1ZMFMsd7d6R-PFju3QpZlb26zbaNcrFf9/view?usp=share_link)

### Guidelines:

1. **Bounding Box**: The bounding box should tightly enclose the cell without cutting any part of it.
2. **Overlapping Cells**: In cases where cells overlap, draw individual bounding boxes for each visible cell.
3. **Avoid Background**: Ensure that the bounding box only contains the cell and as little background as possible.

## 🛠 Tools

For this project, we'll be using the open-source tool [MakeSense](http://makesense.ai).

### Steps to use MakeSense:

1. Visit [MakeSense](http://makesense.ai).
2. Click on `Upload Images` and select the C. elegans images you want to annotate.
3. Define a label, e.g., "C. elegans cell".
4. Start drawing bounding boxes following the guidelines provided.
5. Once done, click on the `Export` button and select the `COCO (JSON)` format.
6. Save the exported JSON annotations locally.

## 📝 How to Contribute

1. **Fork** this repository.
2. **Clone** your forked repository to your local machine.
3. **Create an Issue**: Before starting the annotation, create an issue in the main repository indicating that you're taking up 10 images for annotation. Mention the exact image names in the order they appear in `data.csv` to ensure clarity and avoid overlapping work.
4. Pick the next 10 images in order from the `data.csv` that haven't been annotated yet.
5. Annotate the images using MakeSense and the guidelines provided.
6. Save the annotations in COCO JSON format.
7. Create a new folder with your name (e.g., `JohnDoe/`). Inside this folder, create two subfolders: `images/` and `annotations/`.
8. Place the annotated images in the `images/` folder and the COCO JSON annotations in the `annotations/` folder.
9. Update the `data.csv` file by adding your name next to the images you've annotated.
10. **Commit** your changes with a meaningful commit message.
11. **Push** your changes to your forked repository.
12. Create a **Pull Request** to the main repository with a title like "Annotations by [Your Name]". In the PR description, mention `Close #[Issue Number]` to link and close the issue you created.
13. Once your PR is reviewed and merged, you can pick another set of images to annotate if you wish!

## 🎁 Rewards

- Every valid PR will count towards your Hacktoberfest contributions.
- Top contributors will be acknowledged in the project's documentation and chance for the upcoming gsoc project.

## 🤝 Support

If you have any questions or face any issues, please open an issue in this repository, and we'll get back to you as soon as possible.


Happy annotating and happy Hacktoberfest! 🍂🎉
### How to participate:

Watch this video on Detectron 2 [link](https://www.youtube.com/watch?v=cEgF0YknpZw&t=593s)




