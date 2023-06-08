# Индивидуальная часть итогового проекта по биоинформатике
## Сушкова Дарья Сергеевна, подгруппа 2
### Описание гена
Характеристика | Значение
 --- | --- 
Наименование | WDR5 
Функция | Histone modification read
Комплексы | ATAC, NSL, RING2-L3MBTL2, MLL1/2, MLL3/4
Домены | WD40 super family, CaiC super family, PHA03247 super family   
#### Статья №1
_<ins>Наименование:</ins>_ "WDR5 associates with histone H3 methylated at K4 and is essential for H3 K4 methylation and vertebrate development"   
_<ins>DOI:</ins>_ 10.1016/j.cell.2005.03.036   
_[Ссылка](https://www.cell.com/cell/fulltext/S0092-8674(05)00355-7?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS0092867405003557%3Fshowall%3Dtrue)_   
В статье представлена информация о связи гена WDR5 с эпигенетической меткой H3K4: **_"... the WD40-repeat protein WDR5, directly associates with histone H3 di- and trimethylated at K4 and with H3-K4-dimethylated nucleosomes. WDR5 is required for binding of the methyltransferase complex to the K4-dimethylated H3 tail as well as for global H3 K4 trimethylation and HOX gene activation in human cells."_**   
Результаты данного исследования заключаются в том, что белок с повтором WD40 действует как модуль для распознавания специфической модификации гистонов и предполагает механизм считывания и записи эпигенетической метки для активации генов.   
#### Статья №2
_<ins>Наименование:</ins>_ ""   
_<ins>DOI:</ins>_    
_[Ссылка]()_   
### Множественное белковое выравнивание
Выравнивание гистонов проивзодилось с помощью программы MegaX, которая позволяет визуализировать результат. Использовался метод ClustalW с настройками по умолчанию. Ниже приведены скриншоты для каждого из гистонов. Также в папке /alignments данного репозитория находятся соответствующие FASTA файлы выравниваний гистонов. 
#### H2A
![image](https://github.com/DaryaSushkova/hse23_bio_project/assets/89806836/4171a942-257c-4819-8570-ffba8a537319)
#### H2B
![image](https://github.com/DaryaSushkova/hse23_bio_project/assets/89806836/c5135077-41ec-4b1c-af40-b2514219014e)
#### H3
![image](https://github.com/DaryaSushkova/hse23_bio_project/assets/89806836/bc62e65e-cdb9-4c7f-8f9d-d61ec25cb25e)
#### H4
![image](https://github.com/DaryaSushkova/hse23_bio_project/assets/89806836/0595747d-41c6-44c7-b5ad-6f171501afbe)
### Таблицы E-value
Таблицы генерировались с помощью кода на языке Python. Ноутбук доступен по [ссылке](https://colab.research.google.com/drive/1vqmLLlEZF0UO8zmo2MsQVtyRNV5I4RRI?usp=sharing), а также в папке src данного репозитория.
#### Реальные значения E-value
![image](https://github.com/DaryaSushkova/hse23_bio_project/assets/89806836/7c31c5c6-e719-483f-829a-adb93116ff4b)   
Из таблицы видно, что есть организмы (бактерии и археи), для которых $e-value>1$. В таких случаях вероятность того, что последовательности не гомологичны, становится весьма существенной, поэтому нужно смотреть на другие параметры белков.  
#### Логарифм E-value
![image](https://github.com/DaryaSushkova/hse23_bio_project/assets/89806836/d36375fb-0d95-4826-b822-f1fce102aba9)
### Тепловая карта
Код создания карты также расположен в ноутбуке Google Colab.   
![image](https://github.com/DaryaSushkova/hse23_bio_project/assets/89806836/017ae08d-4e55-46be-8f01-25d71df7ca7f)   
### Вывод
Исходя из получишвихся значений e-value, наиболее дальний гомолог впервые появился в $yeast$ (дрожжи - одноклеточные грибы). Это белок NP_009734.1 (ген SWD3), для которого $e-value=1.22e-46<1e-10$ и разница в длине составляет $334-315=19\ а.о.<100\ а.о.$ Вероятнее всего, белок появился в период одноклеточных эукариот, так как для бактерий и архей выдача blast не говорит о наличии гомологов.
