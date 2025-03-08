# Content-Based Video Retrieval (Multimodal Approach)

## Overview
This project explores a **multimodal framework** that bridges the gap between natural-language user queries and video collections. By combining **advanced vision models** for scene and object detection with **automated captioning**, we attain a deeper semantic understanding of video content. We also employ **query augmentation** using large language models to handle diverse user phrasings more effectively.

## Team
- **Diaeddin Tahboub (1200136)**
- **Ahmad Zubaidia (1200105)**
- **Hamza Najar (1192605)**

**Supervisor**:  
- **Dr. Aziz Qaroush**

This work was carried out for our B.Sc. in Computer Systems Engineering at Birzeit University, Faculty of Engineering & Technology, Department of Electrical & Computer Engineering.

---

## Key Components
1. **Frame Extraction**  
   - Uniform Down-sampling, Scene Detection, or All-Frames processing to capture relevant content.

2. **Feature Representation**  
   - **Visual Embeddings** using CLIP ViT-B/32  
   - **Captioning & Text Embeddings** with mPLUG-Owl, then encoded via CLIP’s text encoder

3. **Fusion Strategies**  
   - Merging visual and textual features (feature-based or score-based) to improve retrieval accuracy.

4. **Query Augmentation**  
   - Generating semantically diverse query variations via large language models (e.g., GPT-3.5).

5. **Ranking Methods**  
   - Handling multiple ground-truth captions per video with techniques like median, medoid, or random ranking.

---

## Datasets
- **MSVD (Microsoft Video Description)**  
  Contains short video clips, each with multiple textual descriptions.

- **MSR-VTT (Microsoft Research Video-to-Text)**  
  A larger dataset featuring more complex video segments, each with multiple captions.

These datasets enable evaluation using metrics like **Recall@k**, **Median Rank**, and **Mean Rank** for robust testing.

---

## Experiment Results

All experimental results, including metrics and logs for different configurations, can be accessed through the following link:  
[**Primary Results Folder**](https://drive.google.com/drive/folders/10u6yGm1jATwtbt9MHldQcJsHXSoPn1yP?usp=sharing)

If the primary link is unavailable, please use our secondary folder link:  
[**Alternate Results Folder**](https://drive.google.com/drive/folders/1IRz_iiRZJS3E2ov1uIJAXDZYV7XnbETW?usp=sharing)


## Results & Discussion
- **Scene-based segmentation** helps in more complex videos, but uniform down-sampling can be sufficient for shorter clips.
- **Multimodal fusion** consistently outperforms single-modality approaches.
- **Augmented queries** increase recall by covering a broader range of phrasing variations.
- **Ranking methods** such as medoid or median can handle multiple captions more effectively, especially for extensive datasets.

---

## Project Presentation
For a detailed walkthrough of the system design and findings, please refer to our **Canva presentation**:
[**Presentation on Canva**](https://www.canva.com/design/DAGcp8V_GJQ/20btkHikAX-ZL_i8Amf5eQ/edit?utm_content=DAGcp8V_GJQ&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

---
## Full Research and Report

A comprehensive write-up of our methodology, experiments, and findings can be found in our full research paper at the link below:  
[**Full Research & Report**](https://drive.google.com/file/d/1PJ5YV2wEMmJEgxVI9bZde0XpBWI0w_zo/view?usp=sharing)

---

## Future Directions
- **Temporal Reasoning**: Adopting video-centric transformers for long-sequence action analysis.  
- **Adaptive Fusion**: Dynamically adjusting modality weights based on query context.  
- **User Interaction**: Extending query augmentation to multilingual queries and personalized user histories.




![ezgif-14bc654194cd56](https://github.com/user-attachments/assets/637671b9-a610-4678-bc7f-2bcca21f5d59)

![ezgif-144cfa1ff4bb5c](https://github.com/user-attachments/assets/f48a0b89-156a-4725-a5e6-4c0ed1cf7954)

![image](https://github.com/user-attachments/assets/527cf039-083c-414a-af3f-38b9545bf340)



