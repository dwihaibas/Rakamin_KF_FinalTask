# Rakamin_KF_FinalTask
SELECT 
  branch_id, 
  provinsi, 
  branch_category, 
  branch_name, 
  RANK() OVER (PARTITION BY provinsi ORDER BY branch_name) AS rating
FROM `rakamin-kf-analytics-418914.dataset_form.kantor cabang kf` 
LIMIT 5


SELECT COUNT(price) AS total_price
FROM `rakamin-kf-analytics-418914.dataset_form.product kf` 
LIMIT 10
