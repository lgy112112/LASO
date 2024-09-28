# code for LASO: Language-guided Affordance Segmentation on 3D Object
here is the link to dataset: https://drive.google.com/file/d/1P4CwQeSALtUOgzhg1ILCiKovE-tcXlSu/view?usp=sharing
The anno_{split}.pkl contains following entries for each sample: 

{'shape_id': 'eaf5e442ac99123c760858b697ef756f',
 'class': 'door',
 'affordance': 'open',
 'mask': array([0., 0., 0., ..., 0., 0., 0.], dtype=float32)}

 The object_split.pkl contains 3D infor mation for each object.

 ---

# LASO

## 如何运行这个Repo

1. **下载数据集**  
   - 打开 `LASO/data_get.ipynb`，并按照说明下载数据集。

2. **修改数据集路径**  
   - 在 `LASO/data_utils/shapenetpart.py` 中找到以下代码：
     ```python
     data_root='/teamspace/studios/this_studio/LASO_dataset'  # dataset path
     ```
   - 将 `'data_root'` 修改为你下载的数据集的绝对路径。

3. **运行训练脚本**  
   - 运行 `LASO/train.sh` 开始训练：
     ```bash
     ./LASO/train.sh
     ```

4. **可视化**  
   - 使用 `LASO/infer_visualize.ipynb` 进行结果可视化。


