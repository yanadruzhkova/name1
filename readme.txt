1. ������� ������� DeepFashion 
http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion/AttributePrediction.html

��������� �������� �������� ��������� �������:
---Anno
------list_attr_cloth.txt
------list_attr_img.txt
------list_bbox.txt
------list_category_cloth.txt
------list_category_img.txt
------list_landmarks.txt
---Eval
------list_eval_partition.txt
---Img
------img

���������� �������� ��� ��������� ����� � fashion_data/

2. ������� ������� ��� ������
�������� ����������� �����, ����� ����� �������������� ���� ��� ������� �����������. �������� �� ��� �������� � �������� ������ ����� dataset.
��� �������:
python dataset_create.py

3. �������� �������� ������
python train.py

4. ������������� ��� ������ �� ���������� � ������ �������, ��� ��� ���������. 
python predict.py