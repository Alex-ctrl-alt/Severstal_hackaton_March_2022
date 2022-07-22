# Severstal-hackaton-march-2022
## As a team member of JEDAI team took 3rd place


## **Task**
 
- Data analysis of given data, contractor debt prediction, feature generation;  
- As result: understandable for the analyst, for the business owner Jupyter Notebook with detailed Exploratory Data Analysis (EDA) and reproductible code of EDA, feature generation, ML, outputs;  


Hackaton webiste:  
https://serverchallenge.ru/ 

Link to notion with task description & data:  
https://russianhackers.notion.site/4-36f74cb0191d4bb19de1709c9633dd89


## **Structure of the repository**
- notebooks - папка для ноутбуков с решениями  
- 0_data_prepare.ipynb - ноутбук где обрабатываются и объединяются данные и выгружаются в pkl  
- auto_eda.ipynb - авто EDA  
- 2_lama_2.ipynb - Light Auto ML решение  
- 7_model_tatget_log_exp_metric_another_reg.ipynb - лучшее решение после окончания хакатона (с логарифмированием и регуляризацией параметром reg_lambda (скор: 0.5423 / 0.5391)  
- submits - папка для хранения сабмитов (csv-файл + ноутбук в zip-архиве)  
- presentations.md - некоторые наиболее интересные скриншоты презентаций топ-7 участников.  



## **Lesson learned (what we could do more)**
- наибольший скор дали переобученные неглубокие модели. Вопрос, как распознать такие случаи?  
- логарифмировть скошеное распределение таргета - попробовал после окончания в песочниуе. Метрика выросла на 0,024!!!  
- модели обучать можно не только последоватьельно (сначала температуру, а потом углерод), но и  
- температуру предсказывать с углеродом и наоборот  
- по 2 раза - сначала без углерода и температуры, а потом прогноз с ними  
- LightAutML в режиме CatBoost+Optuna  
- Тюнинг гиперпараметров (Optuna)  
- стратификацию  
- стекинг и блендинг (можно было воспользоваться шаблоном от Дьяконова)  
- Регуляризацию надо было делать lambda и alpha, а не Только n_trees.  

## **Diploma of the 3rd place**

![image](https://user-images.githubusercontent.com/81492683/180475697-bcbcdd44-fe27-4b5e-8427-062c930dfe2a.png)



