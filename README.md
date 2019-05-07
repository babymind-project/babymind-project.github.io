# How to friendsqa.github.io

### About | Paper | People
#### Source : index.md
###### 1. About
>위치 : **index.md**
> ```
> <div class="about content-container">
>  <h1 class = "content-title">
>   {{ 제목 }}
>  </h1>
>  <p class="content-item">
>   {{ 내용 }}
>  </p>
> </div>
> ``` 

###### 2. Paper
>위치 : **index.md**
> ```
> <div class="papers content-container">
>  <h1 class = "content-title">
>    Paper
>  </h1>
>  <p class="content-item">
>   {{ 논문제목 1 }} <br>
>  <span id="authors"> {{ 저자 }} </span>
>  </p>
>  <p class="content-item">
>   {{ 논문제목 2 }} <br>
>  <span id="authors"> {{ 저자 }} </span>
>  </p>
>  ...
></div>
> ``` 

###### 3. People
> 위치 : **_data/people.yml**
> ``` 
> - name: {{ 이름 }}
> 	affiliation: {{ 직위 }}
> 	src: {{ 이미지 경로 }}
> 	```

***

### Dataset > Overview
#### Source : overview.md
###### 1. Overview
>위치 : **overview.md**
> ```
>  <div class="content-item">
>    <table id="overview">
>      <tr>
>        <th>Training set</th> // Training set header
>        <th>Validation set</th> // Validation set header
>        <th>Test set</th> // Test set header
>      </tr>
>      <tr>
>        <td>training 0</td> // Traing set 0번
>        <td>validation 0</td> // Validation set 0번
>        <td>test 0</td> // Test set 0번
>      </tr>
>      ...
>      ...
>    </table>
>  </div>
> ``` 

***

### Dataset > Explore
#### Source : explore.md
###### 1. Explore

###### 1.1. 왼쪽 상단 (Stats field)
> ```
>    <div class="stats-field">
>      <div id="stats-questions">
>        <span id="header">
>          {{ 질문 개수 }}
>        </span>
>        <ul> 
>          <li>{{ What }}</li>
>          <li>{{ Who }}</li>
>          <li>{{ Where }}</li>
>          <li>{{ Why }}</li>
>          <li>{{ How }}</li>
>        </ul>
>      </div>
>      <div id="stats-episodes">
>        <span id="header">
>          {{ 에피소드 개수 & TV show 개수 }}
>        </span>
>        <ul> 
>          <li> {{ 분야 }}
>            <ul>
>              <li>{{ 제목 }}</li>
>               ...
>            </ul>
>          </li>
>          ...
>        </ul>
>      </div>
> ``` 
###### 1.2. 왼쪽 하단 (Usage field)
>위치 : **explore.md**
> ```
>      <div id="stats-usage">
>        <span id="header"> {{ 제목  }} </span>
>        <p>
>         {{ 내용 }}
>        </p>
>      </div>
> ```
###### 1.3. 오른쪽 상단 (Video field)
>위치 : **explore.md**
> ```
>    <div class="video-field">
>      <video class="viewer" width="100%" height="auto" controls>
>        <source src="{{ video 경로 }}" type="video/{{ video 확장자 }}">
>      </video>
> ```
###### 1.4. 오른쪽 하단 (Question field)
>위치 : **_data/questions.yml**
> ```
>- question: {{ 질문 }} 
>  answer: {{ 정답 번호; 0... }}
>  answers: 
>    - answer: {{ 보기 0 }}
>    - answer: {{ 보기 1 }}
>    ...
> ```

***

### Dataset > Download
#### Source : download.md
###### 1. Annotation Format
>위치 : **download.md**
> ```
><div class="download content-container">
>  <h1 class = "content-title">
>    Download FriendsQA Dataset
>  </h1>
>  <div class = "content-subcontainer">
>    <h2 class="content-subtitle">
>      1. Annotation Format
>    </h2>
>    <div class="content-item">
>      <div class="dataset-field">
>        {% highlight {{ 언어 종류 }} %}
>           {{ 코드 }}
>        {% endhighlight %}
>      </div>
>    </div>
>  </div>
> ``` 
###### 2-4. Descriptions | Video Features | Video Frames
>위치 : **download.md**
> ```
>    <p class="content-item">
>      Download link: 
>      <a id="download_link" href="{{ 다운로드 링크 }}">{{ 표시 내용 }}</a>
>    </p>
> ```

### Dataset > Code
>위치 : **_data/menu.yml**
> ```
> ...
> - name: Dataset
>  child: true
>  children : 
>  - name: Overview
>    link: /dataset/overview
>  - name: Explore
>    link: /dataset/explore
>  - name: Download
>    link: /dataset/download
>  - name: Code  // !!! CODE !!!
>    link: {{ 링크 }} 
>...
> ```

***

### Challenge > 2019
#### Source : challenge_2019.md
###### 1-2. Overview | Important Dates
>위치 : **challenge_2019.md**
>위의 내용 참고.
###### 3. Evaluation
>위치 : **challenge_2019.md**
> ```
>  <div class = "content-subcontainer">
>    <h2 class = "content-subtitle">
>      3. Evaluation
>    </h2>
>    <p class="content-item">
>      Evaluation server link : 
>        <a id="download_link" href="{{ 링크 }}">{{ 표시 내용 }}</a>
>    </p>
>  </div>
> ```
###### 4. Prize
>위치 : **challenge_2019.md**
>위의 내용 참고.
###### 5. Challenge Guidelines
>위치 : **challenge_2019.md**
> ```
>  <div class = "content-subcontainer">
>    <h2 class = "content-subtitle">
>      5. Challenge Guidelines
>    </h2>
>    <p class="content-item">
>      1. {{ 내용 }} <br>
>      2. {{ 내용 }} <br>
>      ...
>    </p>
>  </div>
> ```
###### 6. Organizers
>위치 : **_data/challengeOrganizers2019.yml**
> About > 3. People과 동일.

***

### Workshop > 2019
#### Source : workshop_2019.md**
###### 1-2. Overview | Schedule
>위치 : **workshop_2019.md**
>위의 내용 참고.
###### 3. Invited Speakers
>위치 : **_data/workshopInvitedSpeakers2019.yml**
> About > 3. People과 동일.
###### 4. Organizers
>위치 : **_data/workshopOrganizers2019.yml**
> About > 3. People과 동일.

***

### Sponsor
#### Source : sponsor.md
>위치 : **_data/sponsors.yml**
>```
>- type: {{ Sponsor 타입 }}
>  images: 
>    - src: {{ 이미지 경로 }}
>    - src: {{ 이미지 경로 }}
>    ...
>```

***

### Menu 수정
#### Source : _includes/menu.html
> 위치 : **_data/menu.yml**
###### 1. Single menu
>```
>- name: {{ 메뉴 이름 }}
>  child: false 
>  link: {{ 경로 }}
>```
###### 2. Dropdown menu
>```
>- name: {{ 메뉴 이름 }}
>  child: true
>  children : 
>  - name: {{ Dropdown 이름 1 }}
>    link: {{ Dropdown 경로 1 }} 
>  - name: {{ Dropdown 이름 2 }}
>    link: {{ Dropdown 경로 2 }} 
>    ...
>```
***
### Challenge 추가
#### Source : challenge_{{ 연도 }}.md 추가
###### 1-5. Overview | Important Dates | Evaluation | Prize | Challenge Guideline
>내용 : **challenge_2019.md**와 동일.
###### 6. Organizers
>위치 : **_data/challengeOrganizers{{ 연도 }}.yml** 추가.
>내용 : **_data/challengeOrganizers2019.yml**과 동일.

>위치 : **challenge_{{ 연도 }}.md** 수정.
>```
>  <div class = "content-subcontainer">
>    <h2 class = "content-subtitle">
>      6. Organizers
>    </h2>
>    <div class="content-item">
>      {% for person in site.data.challengeOrganizers{{ 연도 }} %}
>        <div class="member">
>          <div class="member-profile">
>            <img class="member-profile" src="{{person.src}}">
>          </div>
>          <div class="member-info member-name">
>            {{ person.name }}
>          </div>
>          <div class="member-info member-position">
>            {{ person.affiliation }}
>          </div>
>        </div>
>      {% endfor %}
>    </div>
>  </div>
>```
##### Menu에 추가
>위치 : **_data/menu.yml**
>```
>- name: Challenge
>  child: true
>  children :
>    - name: 2019
>      link: /challenge/2019
>    - name: {{ 연도 }}
>      link: /challenge/{{ 연도 }}
>```

***
### Workshop 추가
#### Source : workshop_{{ 연도 }}.md 추가
> 위의 내용 참고.
