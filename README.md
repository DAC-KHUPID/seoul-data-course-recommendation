# 데이트 마이닝: 빅데이터 기반 서울 데이트 코스 추천 알고리즘
<div align="center">
<img width="767" alt="Flowchart" src="https://user-images.githubusercontent.com/44253680/85925687-0d5d8900-b8d5-11ea-9e1c-4f13dbf9282f.png">
</div>  

## Introduction <a id="introduction"></a>
#### Needs  <a id="needs"></a> 
&nbsp;&nbsp;&nbsp;&nbsp;빅데이터 기반의 추천 시스템은 오래 전부터 연구되어왔고, 유튜브, 넷플릭스, 왓챠 등 미디어 플랫폼과 인터넷 쇼핑몰에서 좋은 성능을 발휘했으나, 현재 시장에 출시된 데이트 명소를 추천해주는 애플리케이션은 수요가 높음에도 불구하고 빅데이터 기반의 추천 알고리즘을 사용하지 않고 있음을 발견했다. 따라서 본 프로젝트에서는 **머신러닝을 통해 사용자의 취향을 분석**하고 이를 통해 **데이트 코스를 추천해주는 알고리즘을 개발**한다. 이 알고리즘은 **데이트 코스를 결정하는 데에 어려움을 겪었던 커플들에게 도움**을 줄 것이며, **랜덤 데이트 코스라는 재미 요소**도 줄 수 있을 것이다.

#### Goals <a id="goals"></a>
- 정성적 목표   
이 프로젝트의 **최종 결과물은 데이트 취향과 위치를 고려한 데이트 코스 추천 알고리즘**이며 데이트 코스에는 사용자의 취향에 맞춘 맛집/카페, 데이트 명소(유명 방문지, 보드게임 카페, 볼링장, 방탈출 카페 등등), 영화가 포함되어 있다. 또한 데이트를 하고자 하는 지역구를 선택한다면, 이에 대한 **코스 필터링 기능을 제공**하는 것 또한 최종 결과물에 포함되도록 한다.

- 정량적 목표   
정형화된 데이터 셋이 아닌 점과 선행 연구에 대한 오픈소스 프로젝트가 없는 관계로, 선행 연구와 비교한 정량적 목표 설정은 무리가 있다는 점을 인지하였다. 따라서 표본을 모집 후 만족도를 조사하여 **MOS 기법을 바탕으로 만족도를 조사**하는 것을 대체 방안으로 채택하였다. 테스터들은 구글 설문지를 통해 몇가지 문항들에 답변한 후, 메일로 알고리즘이 추천한 데이트 코스 결과를 받고 이후 다시 메일에 첨부된 만족도 조사에 답하게 된다. 만족도 조사는 알고리즘이 추천한 코스에 대한 만족도를 묻는 총 1개의 문항으로, 1점 '매우 불만족한다' 부터 시작하여 5점 '매우 만족한다까지'로 척도를 제시된다.

## Packages
본 프로젝트에서는 다음과 같은 패키지를 활용하였다.
* [tensorflow(1.15.2)](https://github.com/tensorflow/docs/tree/r1.5/site/en/api_docs)
* [scikit-learn(0.22.1)](https://pypi.org/project/scikit-learn/0.22.1/)
* [cornac(1.6.1)](https://pypi.org/project/cornac/)
* [pypapago](https://github.com/Beomi/pypapago)
* [nltk(3.4.5)](https://pypi.org/project/nltk/3.4.5/)
* [gensim(3.8.3)](https://pypi.org/project/gensim/3.8.3/)
* [pandas (1.0.1)](https://pypi.org/project/pandas/1.0.1/)
* [beautifulsoup(4.8.2)](https://pypi.org/project/beautifulsoup4/4.8.2/)
* [selenium(3.141.0)](https://pypi.org/project/selenium/3.141.0/)
* [numpy(1.18.1)](https://pypi.org/project/numpy/1.18.1/)

## Table of contents
  1. [Introduction](#introduction)
     * [Needs](#needs)
     * [Goals](#goals)
  2. [Data crawling](#data_crawling)
     * [EAT](#data_crawling_eat)
     * [GO](#data_crawling_go)
     * [WATCH](#data_crawling_watch)
  3. [Data preprocessing](#data_preprocessing)
     * [Review translation](#review_translation)
     * [Review tokenizing](#review_tokenizing)
  4. [Review clustering](#review_clustering)
  5. [Modeling](#modeling)
     * [Contents Based Filtering](#cbf)
     * [Neural Collaborative Filtering](#ncf)
  6. [Results](#results)
  7. [Conclusion](#conclusion)
  
## Data crawling <a id="data_crawling"></a>
#### Eat <a id="data_crawling_eat"></a>
#### Go <a id="data_crawling_go"></a>
#### Watch <a id="data_crawling_watch"></a>

## Data preprocessing <a id="data_preprocessing"></a>
#### Review translation <a id="review_translation"></a>
#### Review tokenizing <a id="review_tokenizing"></a>

## Review clustering <a id="review_clustering"></a>

## Modeling <a id="modeling"></a>
#### Contents Based Filtering <a id="cbf"></a>
#### Neural Collaborative Filtering <a id="ncf"></a>

## Results <a id="resultes"></a>
* Main code, table, graph, comparison, ...
* Web link

``` C++
void Example(int x, int y) {
   ...  
   ... // comment
   ...
}
```

## Conclusion <a id="conclusion"></a>
&nbsp;&nbsp;&nbsp;&nbsp;이번 프로젝트에서는 서울 내의 맛집/카페, 데이트 명소, 영화를 모두 포함한 데이트 코스 추천 알고리즘을 기획하고 개발하였다. 단일 장소에 대한 추천을 넘어 각 장소들을 조합하여(필터링 등) 데이트 코스로 추천해주었다는 점에 의의가 있으며 위와 같은 결과를 도출하기 위해 어떤 추천 알고리즘을 사용해야 이 주제에서 가장 적합한 추천을 할 수 있을지에 대한 고민을 통해 다양한 추천 알고리즘의 특성 및 활용 방법을 익힐 수 있었다. 또한 최종 추천을 위해 사용되는 자연어 처리/형용사 추출, 형용사 embedding, vector clustering/clustering distance, data normalization, vector 유사도 측정에 대해서도 각각 어떤 방법론들이 있고 어떤 상황에서 사용해야 하는지 등을 찾아보면서 진행했다. 분석에 적합한 방법들에 대해 성능 평가를 동시에 진행하며 최종적인 알고리즘을 완성할 수 있었다.
&nbsp;&nbsp;&nbsp;&nbsp;결과적으로 이번 프로젝트를 통해 추천 시스템의 A-Z를 직접 구현해봄으로써 추천 알고리즘이 어떻게 동작하는지 잘 이해할 수 있었다. 다만, 적용한 추천 알고리즘의 논문이나 내부 로직을 100% 이해하지 못했다는 아쉬움이 있으며, 더 세부적인 논문 이해를 통해 모델링을 정교화한다면 더 좋은 결과를 도출할 수도 있을 것이라 생각하였다.


## Project Schedule
| Contents | March | April |  May  | June  |
|----------|-------|-------|-------|-------|
|  1. 데이터 수집  |       | :heavy_check_mark:      |       |       |
|  2. 데이터 형식 통합  |       |   :heavy_check_mark:    |       |       |
|  3. 리뷰 데이터 자연어 처리  |       |       |   :heavy_check_mark:    |       |
|  4. 장소별 형용사 데이터 셋 생성  |       |       |  :heavy_check_mark:     |       |
|  5. 유저별 형용사 데이터 셋 생성  |       |       |  :heavy_check_mark:     |       |
|  6. Contents Based Filtering(User, Item based)  |       |       |   :heavy_check_mark:    |       |
|  7. Neural Collaborative Filtering  |       |       |    :heavy_check_mark:   |       |
|  8. 1차 최종 알고리즘 모델링  |       |       |  :heavy_check_mark:     |       |
|  9. 최종 알고리즘 모델링  |       |       |       |   :heavy_check_mark:    |
|  10. 테스트용 구글 폼 제작  |       |       |       |  :heavy_check_mark:     |
|  11. 표본을 대상으로 만족도 조사 시행  |       |       |       |  :heavy_check_mark:     |



## Reports
* [Final Report](Reports/Final.pdf)
* [Demo video](Reports/Demo.mp4)

### Contributors

* [김동혁 (경희대학교 산업경영공학과)](https://github.com/LoveDH)
* [류연주 (경희대학교 관광학과)](https://github.com/YeonjuRyu)
* [유정수 (경희대학교 산업경영공학과)](https://github.com/youjeongsue)

