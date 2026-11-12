# smart-waste-classifier
CNN-based waste classification and segregation using PyTorch and Streamlit
## Dataset Quality and Limitations

During duplicate inspection, three groups of identical bottle images were found with conflicting class labels (plastic vs. glass, plastic vs. glass, and glass vs. metal). All six files were excluded to avoid inconsistent labels during model training.

Duplicate detection was performed using MD5 hashing, which detects exact copies but cannot identify near-duplicates such as resized, cropped, or compressed versions of the same image. Therefore, some near-duplicates may remain across dataset splits, potentially resulting in slightly optimistic test performance.
