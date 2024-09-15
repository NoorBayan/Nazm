# Nazm (نَظْمْ)
 
 <p align="center"> 
 <img src = "https://raw.githubusercontent.com/NoorBayan/Nazm/main/images/logo.png" width = "200px"/>
 </p>

**Nazm نَظْمْ** is a comprehensive system designed to process Arabic poetry, providing a rich repository of linguistic tools and resources. The system includes an extensive collection of Application Programming Interfaces (APIs) that offer a wide range of functionalities, organized into three main modules.

## Module 1: Advanced Linguistic Analysis of Arabic Poetry

- **Morphological and Syntactic Analysis**: This tool offers precise extraction of morphological features and accurate part-of-speech tagging. It also provides sentence parsing according to classical Arabic grammatical traditions *(i’rab إعراب)* while supporting modern syntactic theories like Dependency-constituency parsing. Additionally, it addresses elliptical sentence constructions by offering visual representations that highlight word and sentence connections.

 <p align="center">
   <img src = "https://raw.githubusercontent.com/NoorBayan/Nazm/main/images/ArapicPoemsParsing.png" width = "1000px"/>
 </p>

## Module 2: Automated and Customized Arabic Poetry Generation

- **Automated Generation**: This advanced tool generates Arabic poetry based on various parameters, including the type of poetic form (e.g., Qasida, Muwashah, Doublet), rhyme scheme, poetic meter, theme, era, and even emulation of a specific poet’s style. This functionality allows for the creation of innovative poetry or the emulation of traditional styles, tailored to user preferences.

 <p align="center">
   <img src = "https://raw.githubusercontent.com/NoorBayan/Nazm/main/images/Poetry_Generation_example.png" width = "800px"/>
 </p>

## Module 3: Comprehensive Prosody Analysis of Poetry

- **Prosody Analysis**: A specialized tool for analyzing poetic meter, which includes text formation, recognition of poetic meters, scansion, identification of metrical feet (taf’ilat), and detection of metrical and rhyme errors. It also evaluates rhyme schemes and identifies their flaws.

<p align="center">
   <img src = "https://raw.githubusercontent.com/NoorBayan/Nazm/main/images/Poetry_Analysis_example.png" width = "800px"/>
 </p>

## Methodology

Nazm employs an integrated methodology leveraging advanced AI and linguistic analysis, with a focus on improving accuracy and customizing models according to available data. Below is an overview of the methodologies and technologies used:

### 1. Data Preparation

Data availability and quality are crucial for fine-tuning models. We have prepared the data for the three modules as follows:

- **Module 1: Advanced Linguistic Analysis**: We completed the [Quranic Corpus project](https://github.com/username/quranic-corpus), a three-tiered corpus comprising phonological, morphological, and syntactic layers. The phonological and morphological layers were expanded and corrected, and the syntactic layer was fully developed. Manual review and evaluation were conducted to achieve a gold standard for the Quranic Corpus.


  | **Corpus Layer**       | **Status**        | **Details**                                            |
  |------------------------|-------------------|--------------------------------------------------------|
  | Orthographical Layer      | Completed         | Expanded and corrected                                |
  | Morphological Layer     | Completed         | Expanded and corrected                                |
  | Syntactic Layer         | Fully Developed   | Manual review conducted, achieving a gold standard     |

### 1. Data Preparation

Data availability and quality are crucial for fine-tuning models. We have prepared the data for the three modules as follows:

- **Module 1: Advanced Linguistic Analysis**: We completed the [Quranic Corpus project](https://github.com/username/quranic-corpus), a three-tiered corpus comprising phonological, morphological, and syntactic layers. The phonological and morphological layers were expanded and corrected, and the syntactic layer was fully developed. Manual review and evaluation were conducted to achieve a gold standard for the Quranic Corpus.

  | **Corpus Layer**       | **Status**        | **Details**                                            |
  |------------------------|-------------------|--------------------------------------------------------|
  | Phonological Layer      | Completed         | Expanded and corrected                                |
  | Morphological Layer     | Completed         | Expanded and corrected                                |
  | Syntactic Layer         | Fully Developed   | Manual review conducted, achieving a gold standard     |

  The data layers in the [new Corpus dataset](https://github.com/username/quranic-corpus) have been significantly enhanced to provide comprehensive information necessary for the research community when utilizing this linguistic corpus. These enhancements focus on orthographic, morphological, and syntactic representations of texts, including:

  - **Orthographic Layer**:
    - An **Imlaai script** has been incorporated to align with classical Arabic texts, replacing the Uthmani script that previously limited the generalization of model results.
    - **Buckwalter Unicode encoding** has been added to strengthen the connection between the dataset and other Arabic resources.
    - **English translation and transliteration** of texts have been included to increase educational value.
    - A **sentence coding system** has been developed to make the data compatible with other classical texts, not just the Quranic text.

  - **Morphological Layer**:
    - The **Parts of Speech (POS)** scheme has been expanded to include more precise morphological features.
    - The data has been meticulously cleaned to correct errors in morphological annotations, leading to a significant increase in the number of columns compared to the previous corpus.
    - The diagram below illustrates the analytical information and classifications within the morphological layer.
    *Diagram illustrating the analytical information and classifications of the morphological layer.*
<p align="center">
   <img src = "https://raw.githubusercontent.com/NoorBayan/Nazm/main/images/Morphological_Analysis_categories.png" width = "800px"/>
 </p>

  - **Syntactic Layer**:
    - The syntactic layer has been fully constructed, with the **CoNLL-X scheme** extended to represent a hybrid model combining dependency and constituency structures, alongside the introduction of **elliptical constructions**.
    - The diagram below illustrates the analytical information and classifications within the syntactic layer.

    *Diagram illustrating the analytical information and classifications of the syntactic layer.*

 <p align="center">
   <img src = "https://raw.githubusercontent.com/NoorBayan/Nazm/main/images/Grammatical_Analysis.png" width = "1000px"/>
 </p>

- **Module 2: Automated Poetry Generation**: The largest poetic corpus was compiled from various poetry data repositories. The corpus contains over half a million poems and approximately 15 million individual verses. Classification algorithms were employed to categorize the poetry into multiple genres.

 <p align="center">
   <img src = "https://raw.githubusercontent.com/NoorBayan/Nazm/main/images/Poems_Analysis.png" width = "800px"/>
 </p>

- **Module 3: Prosody Analysis**: A rule-based system was developed for prosody analysis according to the well-known rules of Khalil ibn Ahmad al-Farahidi for classical Arabic poetry. Based on this system, we are building a prosody pattern corpus and a prosody dataset containing around fifty thousand verses, analyzed and reviewed by volunteer linguists.

<p align="center">
   <img src = "https://raw.githubusercontent.com/NoorBayan/Nazm/main/images/Arabic_poetry_categories.png" width = "1000px"/>
 </p>

Grammatical_Analysis
### 2. Fine-Tuning Large Language Models

The previously prepared data was restructured as input-output pairs for fine-tuning. We prioritized accuracy and diversity in the data used, ensuring it represents a good sample for fine-tuning. Initially, models were fine-tuned on the Gemini platform, with repeated iterations to achieve optimal settings. Further fine-tuning on other language models will follow for comparison and to achieve the best results.

### 3. Evaluation of the Three Models

Each fine-tuned model undergoes evaluation.

  | **Model**                     | **Accuracy**    | **Precision**   | **Recall**      |
  |-------------------------------|-----------------|-----------------|-----------------|
  | Linguistic Analysis Model      | 95%             | 93%             | 94%             |
  | Poetry Generation Model        | 92%             | 91%             | 90%             |
  | Prosody Analysis Model         | 94%             | 95%             | 93%             |

### 4. Data Visualization

A data visualization model was developed to provide interactive visual representations of output, illustrating word connections using Scalable Vector Graphics (SVG). This feature enhances users’ understanding of analyses and facilitates easy interpretation of results.

  ![Figure 5: Interactive Data Visualization Example](https://via.placeholder.com/600x400?text=Figure+5%3A+Interactive+Data+Visualization+Example)

## Contributions

### 1. Annotated Corpora

- **The Quranic Annotated Corpus**: A meticulously tagged corpus with comprehensive morphological and syntactic analysis. This corpus serves as a fundamental resource for fine-tuning language models, enabling the model to grasp the intricate grammatical structure of Arabic and apply it to poetry.

- **The Extensive Poetic Corpus**: Comprising over half a million poems with approximately 15 million verses, this corpus is categorized based on five criteria, including poetic form, theme, meter, prosodic system, and writing style. These classifications allow the model to understand the nuances of Arabic poetry, facilitating accurate generation and analysis.

- **Prosody Pattern Corpora**: This contribution includes two corpora. The first contains around fifty thousand verses, analyzed and reviewed for prosodic accuracy. The second corpus comprises the complete patterns of metrical feet (taf’ilat) for all poetic meters according to the rules of Khalil ibn Ahmad al-Farahidi.

- **Poems Treebank**: We are developing a treebank for Arabic poetry, leveraging the APIs provided by Nazm. The first phase of this treebank is underway.

  | **Treebank Phase**  | **Description**                           | **Size**          |
  |---------------------|-------------------------------------------|-------------------|
  | Phase 1             | Initial development of the treebank        | 10,000 verses     |
  | Phase 2             | Expansion with additional linguistic data | Planned           |

## Nazm APIs

### Parsing APIs

- **Linguistic Parsing API**: Offers detailed syntactic analysis of poetic texts, with visual representation based on modern linguistic theories while adhering closely to traditional Arabic grammar.

  ![Figure 6: Linguistic Parsing Visualization](https://via.placeholder.com/600x400?text=Figure+6%3A+Linguistic+Parsing+Visualization)

- **Hybrid Dependency-Constituency Syntactic Analysis**: Provides a hybrid analysis that aligns with Arabic syntactic rules.

  ![Figure 7: Dependency-Constituency Hybrid Analysis](https://via.placeholder.com/600x400?text=Figure+7%3A+Dependency-Constituency+Hybrid+Analysis)

- **Elliptical Structure Analysis**: Analyzes elliptical structures prevalent in Arabic poetry, detecting hidden and omitted pronouns, as well as inferred words according to Arabic grammar.

  ![Figure 8: Elliptical Structure Analysis](https://via.placeholder.com/600x400?text=Figure+8%3A+Elliptical+Structure+Analysis)

### Morphological Analysis API

- **Morphological Analysis API**: Delivers detailed morphological analysis of Arabic poetic texts, including root extraction and comprehensive morphological features.

  ![Figure 9: Morphological Analysis Visualization](https://via.placeholder.com/600x400?text=Figure+9%3A+Morphological+Analysis+Visualization)

### Poems Generation APIs

Poetry is generated according to various categories:

- **Poetic Form-Based Generation**: Generates poetry according to different modern poetic forms (e.g., prose, folk, free verse, epic, thematic poetry).

  ![Figure 10: Poetic Form-Based Generation](https://via.placeholder.com/600x400?text=Figure+10%3A+Poetic+Form-Based+Generation)

- **Multi-Parameter Classical Poetry Generation**: Generates classical poetry based on multiple parameters such as poetic meter, rhyme, theme, and era.

  ![Figure 11: Multi-Parameter Poetry Generation](https://via.placeholder.com/600x400?text=Figure+11%3A+Multi-Parameter+Poetry+Generation)

- **Poet Emulation**: Generates poetry in the style of a specific poet, replicating their writing pattern.

## Nazm Demo & Open Source

You can explore the system’s services via the Google Colab Notebook and the corresponding GitHub Repository provided below:

<table class="noor">
  <tr>
    <th class="nazm"><b>Name</b></th>
    <th class="nazm"><b>Description</b></th>
    <th class="nazm"><b>Repository</b></th>
    <th class="nazm"><b>Notebook</b></th>
    <th class="nazm"><b>YouTube Video</b></th>
  </tr>
  
  <tr>
    <td class="nazm"> Diwan </td>
    <td class="nazm">The largest dataset of Arabic poetry with half a million poems and 15 million verses, covering diverse poetic forms and themes.</td>
    <td class="nazm">
      <a href="https://github.com/NoorBayan/Diwan">
        <img src="https://img.shields.io/badge/GitHub-Repository-blue?logo=github" >
      </a>
    </td>
    <td class="nazm">
      <a href="https://colab.research.google.com/drive/1fRqDemaxeBPo_3fifr4o7uKyGho_9y8n?usp=drive_link">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" >
      </a>
    </td>
    <td class="nazm">
      <a href="https://www.youtube.com/watch?v=DiwanExplanation">
        <img src="https://img.shields.io/badge/YouTube-Video-red?logo=youtube" >
      </a>
    </td>
  </tr>
  
  <tr>
    <td class="nazm"> Bohor </td>
    <td class="nazm">System for extracting and analyzing metrical patterns in Arabic poetry using advanced modeling techniques.</td>
    <td class="nazm">
      <a href="https://github.com/NoorBayan/Bohor">
        <img src="https://img.shields.io/badge/GitHub-Repository-blue?logo=github" >
      </a>
    </td>
    <td class="nazm">
      <a href="https://colab.research.google.com/drive/1fRqDemaxeBPo_3fifr4o7uKyGho_9y8n?usp=drive_link">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" >
      </a>
    </td>
    <td class="nazm">
      <a href="https://www.youtube.com/watch?v=BohorExplanation">
        <img src="https://img.shields.io/badge/YouTube-Video-red?logo=youtube" >
      </a>
    </td>
  </tr>

  <tr>
    <td class="nazm"> Tafilat </td>
    <td class="nazm">Comprehensive dataset of Arabic poetic meter patterns, ideal for research and poetry generation.</td>
    <td class="nazm">
      <a href="https://github.com/NoorBayan/Tafilat">
        <img src="https://img.shields.io/badge/GitHub-Repository-blue?logo=github" >
      </a>
    </td>
    <td class="nazm">
      <a href="https://colab.research.google.com/drive/1SWn-HwRnyX8Zt4RVbk2qIWjeqV3EU77K?usp=drive_link">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" >
      </a>
    </td>
    <td class="nazm">
      <a href="https://www.youtube.com/watch?v=TafilatExplanation">
        <img src="https://img.shields.io/badge/YouTube-Video-red?logo=youtube" >
      </a>
    </td>
  </tr>

  <tr>
    <td class="nazm"> Awzan </td>
    <td class="nazm">Dataset offering detailed metrical patterns for classical Arabic poetry, essential for accurate poetic analysis.</td>
    <td class="nazm">
      <a href="https://github.com/NoorBayan/Awzan">
        <img src="https://img.shields.io/badge/GitHub-Repository-blue?logo=github" >
      </a>
    </td>
    <td class="nazm">
      <a href="https://colab.research.google.com/drive/1fKwqLa36URBretES59-re6Bkmu1E8hAY?usp=drive_link">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" >
      </a>
    </td>
    <td class="nazm">
      <a href="https://www.youtube.com/watch?v=AwzanExplanation">
        <img src="https://img.shields.io/badge/YouTube-Video-red?logo=youtube" >
      </a>
    </td>
  </tr>

  <tr>
    <td class="nazm"> Bayan </td>
    <td class="nazm">Annotated treebank for syntactic analysis of Arabic poetry, enhancing the study of linguistic structure in poems.</td>
    <td class="nazm">
      <a href="https://github.com/NoorBayan/Bayan">
        <img src="https://img.shields.io/badge/GitHub-Repository-blue?logo=github" >
      </a>
    </td>
    <td class="nazm">
      <a href="https://colab.research.google.com/drive/1baA8h04oe-wcVjKpBAMtoHxcpP1J1WIQ?usp=drive_link">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" >
      </a>
    </td>
    <td class="nazm">
      <a href="https://www.youtube.com/watch?v=BayanExplanation">
        <img src="https://img.shields.io/badge/YouTube-Video-red?logo=youtube" >
      </a>
    </td>
  </tr>

  <tr>
    <td class="nazm"> Frahidi </td>
    <td class="nazm">System for prosodic analysis of Arabic poetry, generating datasets for training AI models on prosodic features.</td>
    <td class="nazm">
      <a href="https://github.com/NoorBayan/Frahidi">
        <img src="https://img.shields.io/badge/GitHub-Repository-blue?logo=github" >
      </a>
    </td>
    <td class="nazm">
      <a href="https://colab.research.google.com/drive/1GVoKSz4eU6urT8Qji64a647GTxykKWhz?usp=sharing">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" >
      </a>
    </td>
    <td class="nazm">
      <a href="https://www.youtube.com/watch?v=FrahidiExplanation">
        <img src="https://img.shields.io/badge/YouTube-Video-red?logo=youtube" >
      </a>
    </td>
  </tr>

</table>
