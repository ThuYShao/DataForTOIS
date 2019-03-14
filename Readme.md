## Data Description of TOIS paper “On Annotation Methodologies for Image Search Evaluation”

### tasks.txt
This file contains the description of 12 tasks we used in our paper.

### query_satisfaction.csv
1. This file contains users' satisfaction feedback of 1119 queries we used in our paper.
2. The format:
    user_id, task_id, query_id, query, satisfaction

### row_judgments.csv
1. This file contains row-based topical relevance scores of results in the top ten rows for 1119 queries we used in our paper.
2. The format:
    user_id, task_id, query_id, row_id, relevance

### page_judgments.csv
1. This file contains page-based topical relevance scores of results in the first two pages for 1119 queries we used in our paper.
2. The format:
    user_id, task_id, query_id, page_id, relevance

### S100_annotation.tsv
1. This file contains raw S100 topical relevance scores of results in the top ten rows for 1119 queries we used in our paper.
2. The format:
    image_id \t query \t score_list \t worker_list
    ** note ** : image_id is composed of user_id, task_id, query_id, position (row_column), joined by '/'. score_list and worker_list are composed with raw relevance scores annoted for the image and the corresponding workers, respectively. 


### item_info_judgments.tsv
1. This file contains the information (including S4 item-based topical relevance & image quality annotation & S100 annotation) of results in the top ten rows for 1119 queries we used in our paper.
2. The format:
    user_id \t task_id \t query_id \t query \t list_id \t rank \t url \t relevance \t quality \t description \t row \t column \t top \t left \t width \t height \t S100
