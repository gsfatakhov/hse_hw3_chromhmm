# HW 3

#### Фатахов Георгий группа 1


## Выбор клеточной линии

`A549` из ДЗ 2.

## Google Colab
[Ноутбук](https://colab.research.google.com/drive/1C0gnj4HhXcmwJR75Hrx8rILGcrE2SNn6?usp=sharing)

## Выбранные Гистоновые Метки

### Соответствие меток файлам
Метка | Файл
--- | ---
H3K4me2 | wgEncodeBroadHistoneA549H3k04me2Dex100nmAlnRep1.bam
H3K79me2 | wgEncodeBroadHistoneA549H3k79me2Dex100nmAlnRep1.bam
H3K36me3 | wgEncodeBroadHistoneA549H3k36me3Dex100nmAlnRep1.bam
H4K20me1 | wgEncodeBroadHistoneA549H4k20me1Etoh02AlnRep1.bam
H3K9me3 | wgEncodeBroadHistoneA549H3k09me3Etoh02AlnRep1.bam
H3K4me1 | wgEncodeBroadHistoneA549H3k04me1Dex100nmAlnRep1.bam
H3K27ac | wgEncodeBroadHistoneA549H3k27acDex100nmAlnRep1.bam
H3K9ac | wgEncodeBroadHistoneA549H3k09acEtoh02AlnRep1.bam
H3K4me3 | wgEncodeBroadHistoneA549H3k04me3Dex100nmAlnRep1.bam
H3K27me3 | wgEncodeBroadHistoneA549H3k27me3Dex100nmAlnRep1.bam


## Получение фалйа `cellmarkfiletable.txt`
#### Клеточная линия 
A549

#### Файлы гистоновых меток
Название метки + `.bam`

#### Файл с контролем 
`ControlDex100AlnRep1.bam`


## ChromHMM

### Emission
![Image](/data/emissions_15.png)

### Overlap
![Image](/data/A549_15_overlap.png)

### Transition 
![Image](/data/transitions_15.png)

### RefSeqTSS
![Image](/data/A549_15_RefSeqTSS_neighborhood.png) 

### RefSeqTES
![Image](/data/A549_15_RefSeqTES_neighborhood.png)

## Эпигенетические Типы

- Active Promoter
  - *Маркеры*: H3K27me3, H3K4me3, H3K4me2
  - *Локализация*: интроны или экзоны
  - *Картинка*: ![Image](/data/picture_1.png)

- Weak Enhancer/Weak Transcribed
  - *Маркеры*: H3K4me2, H3K4me1
  - *Локализация*: часто в RefSeqTES, RefSeqGene, у ядерной ламины
  - *Картинка*: ![Image](/data/picture_2.png)

- Strong Enhancer/Transcriptional Elongation
  - *Маркеры*: H3K9ac, H3K27ac, H3K4me3, H3K4me2, H3K4me1
  - *Локализация*: часто в RefSeqTES, RefSeqTSS2Kb, у ядерной ламины
  - *Картинка*: ![Image](/data/picture_3.png)

- Active Promoter
  - *Маркеры*: H3K9ac, H3K27ac, H3K4me3, H3K4me2
  - *Локализация*: часто в CpGIslands, RefSeqTES, RefSeqExon, RefSeqTSS2Kb
  - *Картинка*: ![Image](/data/picture_4.png)

- Active Promoter
  - *Маркеры*: H3K9ac, H3K27ac, H3K4me3, H3K4me2
  - *Локализация*: часто в RefSeqTES, RefSeqTSS2Kb, RefSeqExon, CpGIslands, RefSeqGene
  - *Картинка*: ![Image](/data/picture_5.png)

- Weak Enhancer
  - *Маркеры*: H3K79me2, H3K9ac, H3K27ac, H3K4me3, H3K4me2
  - *Локализация*: часто в RefSeqGene, RefSeqTES, иногда в RefSeqExon
  - *Картинка*: ![Image](/data/picture_6.png)

- Weak Enhancer
  - *Маркеры*: H3K9ac, H3K27ac, H3K4me1
  - *Локализация*: часто в RefSeqTES
  - *Картинка*: ![Image](/data/picture_7.png)

- Weak Enhancer
  - *Маркеры*: H3K4me1
  - *Локализация*: часто в RefSeqTES, иногда у ядерной ламины
  - *Картинка*: ![Image](/data/picture_8.png)

- Weak Enhancer
  - *Маркеры*: H3K79me2, H3K4me1
  - *Локализация*: часто в RefSeqGene, иногда в RefSeqTES и RefSeqExon
  - *Картинка*: ![Image](/data/picture_9.png)

- Weak Transcribed
  - *Маркеры*: H3K79me2
  - *Локализация*: часто в RefSeqGene
  - *Картинка*: ![Image](/data/picture_10.png)

- Weak Transcribed
  - *Маркеры*: H3K36me3, H3K79me2
  - *Локализация*: часто в RefSeqGene, иногда в RefSeqTES и RefSeqExon
  - *Картинка*: ![Image](/data/picture_11.png)

- Weak Transcribed
  - *Маркеры*: H3K36me3
  - *Локализация*: часто в RefSeqGene, иногда в RefSeqTES и RefSeqExon
  - *Картинка*: ![Image](/data/picture_12.png)

- Repressed
  - *Локализация*: преимущественно на ядерной ламине, в области репрессированного гетерохроматина
  - *Картинка*: ![Image](/data/picture_13.png)

- Heterochromatin
  - *Маркеры*: H3K27me3
  - *Локализация*: преимущественно на ядерной ламине, в области репрессированного гетерохроматина
  - *Картинка*: ![Image](/data/picture_14.png)

- Heterochromatin
  - *Маркеры*: H3K9me3
  - *Локализация*: преимущественно на ядерной ламине, в области репрессированного гетерохроматина
  - *Картинка*: ![Image](/data/picture_15.png)


 ## Бонус
 ```
state_names = [ 'Active_Promoter',
                'Weak_Enhancer',
                'Strong_Enhancer',
                'Active_Promoter',
                'Active_Promoter',
                'Weak_Enhancer',
                'Weak_Enhancer',
                'Weak_Enhancer',
                'Weak_Enhancer',
                'Weak_Transcribed',
                'Weak_Transcribed',
                'Weak_Transcribed',
                'Repressed',
                'Heterochromatin',
                'Heterochromatin' ]

with open(f'data/A549_15_dense.bed', 'r') as origin_file:
  with open(f'A549_15_dense_named.bed', 'w') as named_file:
    lines = origin_file.readlines()
    named_file.write(lines[0])
    for line in lines[1:]:
        line_splited = line.split('\t')
        line_splited[3] += '_' + state_names[int(line_splited[3]) - 1]
        named_file.write('\t'.join(line_splited))
 ```
Результат в папке data