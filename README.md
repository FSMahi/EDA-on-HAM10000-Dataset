# 🩺 Exploratory Data Analysis (EDA) on HAM10000 Skin Cancer Dataset

This project performs an in-depth exploratory data analysis (EDA) on the **HAM10000** dataset — a collection of 10,000 dermatoscopic images of common pigmented skin lesions. The goal is to uncover meaningful patterns, handle missing values, and prepare the dataset for further machine learning applications such as lesion classification.

---

## 📁 Dataset Description

The **HAM10000** dataset (`Human Against Machine with 10000 training images`) is publicly available and used extensively for skin cancer classification. It includes:

- Over **10,000** dermoscopic images.
- Metadata: `age`, `sex`, `localization`, `dx`, `dx_type`, etc.
- Seven skin lesion categories:
  - akiec – Actinic keratoses
  - bcc – Basal cell carcinoma
  - bkl – Benign keratosis-like lesions
  - df – Dermatofibroma
  - mel – Melanoma
  - nv – Melanocytic nevi
  - vasc – Vascular lesions

---

## 📊 Exploratory Analysis Steps

### 1. ✅ **Initial Data Inspection**
- Loaded the metadata CSV.
- Checked for missing values and data types.
- Displayed unique values in critical columns.

### 2. 🧼 **Missing Value Handling**

### 3. ⚖️ **Class Imbalance Check**
- Visualized the class distribution of `dx` using bar plots.
- Insights: Heavy imbalance — e.g., ‘nv’ dominates while others are underrepresented.

### 4. 🔍 **Demographic Analysis**
- Age distributions across lesion types and genders using violin and box plots.
- Gender distribution per lesion type and body part.
- Created age groups (bins) and analyzed frequency.

### 5. 📍 **Body Location vs. Lesion Type**
- Analyzed most common locations for each lesion type using stacked bar plots.

### 6. 🧪 **Diagnosis Method (`dx_type`)**
- Counted methods like histopathology, consensus, etc.
- Compared diagnosis method vs. lesion type.

### 7. ❓ **Unique Lesion Analysis**
- Counted number of unique `lesion_id`.
- Visualized how many images are associated with each lesion ID.

---

## 📁 CSV Files Explained

| File Name                  | Description |
|---------------------------|-------------|
| `HAM10000_metadata.csv`   | Primary metadata for each image (used in EDA) |
| `hmnist_28_28_RGB.csv`    | Flattened RGB image pixel data (28x28x3) for ML pipelines |
| `hmnist_28_28_L.csv`      | Grayscale version of image pixels (28x28) |
| `hmnist_8_8_RGB.csv`      | Downsampled image version (8x8x3) |
| `hmnist_8_8_L.csv`        | Grayscale, 8x8 version |
| `HAM10000_images_part_1/2`| Image folders (used for visualization and classification tasks) |

---

## 🛠 Future Work

- ✅ Complete preprocessing for balanced datasets.
- ✅ Enhance visualization with image samples.
- ⏳ Apply ML models (CNN, ViT, CapsNet) on preprocessed data.
- ⏳ Implement segmentation + classification pipeline.

---

## 📚 Technologies Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Jupyter Notebook

---


## 📄 License

This project is open-source under the MIT License. See the `LICENSE` file for more details.
https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000

