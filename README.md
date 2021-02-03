# chapter2 알고리즘 기초

## topic1 입력한 자료를 출력하려면 어떤 과정이 필요할까요?

### 알고리즘

- 컴퓨팅은 입력을 받아 그 입력을 처리한 후 출력하는 과정입니다. 알고리즘은
  입력에서 받은 자료를 출력형태로 만드는 처리 과정을 뜻합니다. 즉, 알고리즘이란 입력값을 출력값의 형태로 바꾸기 위해 어떤 명령들이 수행되어야 하는지에 대한 규칙들의 나열 방법을 따라 알고리즘의 종류가 달라집니다. 같은 출력값이라도 알고리즘적 순서 나열에 따라 출력값에 도달하는 시간은 서로 다를 수 있습니다.

### 정확한 알고리즘(정확성)

- 알고리즘은 입력을 출력으로 바꾸기 위해 컴퓨토거 따르는 일련의 절차입니다. 알고리즘은 우리의 일상생활 언어로도 표현할 수 있습니다.

### 효율적인 알고리즘(효율성)

- 더 직관적이고 효휼적인 알고리즘이 뭐가 있을지 생각해봅니다. 전화번호부를 가운데를 폅니다 Mike가 그 페이지에 있다면 우리 알고리즘은 끝납니다. 없다면, 전화번호부가 이름순으로 정렬되어 있으므로 우리는 Mike가 지금 페이지보다 앞부부분에 있는지 뒷부분에 있는지 알로 있습니다. 그러므로 책의 절반을 버릴 수 있게 되고 나머지 절반에 대한 똑같은 알고리즘을 수행합니다. 합 페이지가 남을 때까지 계속 수행합니다. 마지막에 남은 한페이지에는 Mike의 이름이 있거나 없거나 둘 중 하나일 겁니다.

## topic2 알고리즘을 이해하기 쉽게 표현하는 방법이 있을까요?

### 의사 코드

- 컴퓨터 프로그램은 프로그래밍 언어로 작성됩니다. 프로그래밍 언어는 일반적으로 기계가 알아들을 수 있도록 명령을 내리기 위해 사용되는 언어입니다. 프로그래밍 언어는 특정한 문법에 의해 작성된 코드를 요구합니다. 알고리즘을 표현하는 방법으로는 자연어(natural language), 의사 코드(Pseudocode), 순서도(flowchart)등이 있습니다. 의사 코드는 프로그래밍 언어보다 문법적 제약을 적게 받으므로 알고리즘 표현에 많이 사용됩니다.

### 의사 코드의 요소

- 의사 코드를 작성하는 올바른 방법이란 없습니다. 어떤 때에는 당신의 목적이 무엇인가에 따라 의사 코드가 더 자세할 수도있습니다. 프로그래밍 언어와는 다르게, 의사 코드를 어떻게 작성해야 하는지를 정의한 문법은 없습니다. 그러나 의사 코드에는 자주 사용되는 몇 가지 요소들이 있습니다. 위의 예시에서 볼 수 있는 것처럼 의사 코드에는 값을 할당한다는 개념이 종종 사용됩니다. 의사 코드에는 반복문(어떤 조건 하에서 특정 명령문이 반복되어 실행되는 것)이나 조건문(특정 조건으로 명령이 실행되기도 하고 건너뛰기도 하는 것)을 포함하기도 합니다. 의사 코드에서 사용될 수 있는 이런 개념들은 프로그래밍 언어로 작성된 프로그램에서 중요한 개념입니다. 프로그래밍 언어를 배운 후에도 의사 코드는 문법 걱정 없이 알고리즘을 단계별로 표현할 수 있는 유용한 방법이며 프로그램의 논리를 이해하는데 더 효과적인 방법이다.

## topic3 자료를 맨 처음부터 하나씩 비교하면서 찾는 방법은 무엇이라고 하나요?

### 선형 탐색

- 찾고자 하는 자료를 탐색하는 데 사용되는 다양한 알고리즘이 있습니다. 그 중 하나가 선형 탐색입니다. 선형탐색은 원하는 원소가 발견돨 때까지 처음부터 마지막 자료까지 차례대로 탐색합니다. 이렇게 하여 선형 탐색은 찾고자 하는 자료를 찾을 때까지 모든 자료를 확인해야 합니다.

### 효율성 그리고 비효율성

- 선형 탐색 알고리즘은 정확하지만 아주 효율적이지 못한 방법입니다. 리스트의 길이가 n이라고 했을 때, 최악의 경우 리스트의 모든 원소를 확인해야 하므로 n번만큼 실행됩니다. 여기서 최악의 상황은 찾고자 하는 자료가 맨 마지막에 있거나 리스트 안에 없는 경우를 말합니다. 만약 100만 개의 원소가 있는 리스트라고 가정해본다면 효율성이 매우 떨어짐을 느낄 수 있습니다. 반대로 최선의 상황은 처음시도했을 때 찾고자 하는 값이 있는 경우입니다. 평균적으로 선형 탐색이 최악의 상황에서 종료되는 것에 가깝다고 가정할 수 있습니다. 선형 탐색은 자료가 정렬되어 있지 않거나 그 어떤 정보도 없어 하나씩 찾아야 하는 경우에 유용합니다. 이러한 경우 무작위로 탐색하는 것보다 순서대로 탐색하는 것이 더 효율적입니다. 이제 여러분은 왜 탐색 이전에 정렬해줘야 하는지 알 수 있을 것입니다. 정렬은 시간이 오래 걸리고 공간을 더 차지합니다. 하지만 이 추가적인 과정을 진행하면 여러분이 여러 번 리스트를 검색해야 하거나 매우 큰 리스트를 검색해야 할 경우 시간을 단축할 수 있을 것입니다.

## topic4 인접한 두개의 자료를 차례로 비교하면서 정렬하는 것을 무엇이라고 하나요?

### 버블 정렬

- 정렬되지 않은 리스트를 탐색하는 것 보다 정렬한 뒤 탐색하는 것이 더 효율적입니다. 정렬 알고리즘 중 하나는 버블 정렬입니다. 버블 정렬은 두 개의 인접한 자료 값을 비교하면서 위치를 교환하는 방식으로 정렬하는 방법을 말합니다. 버블 정렬은 단 두 개의 요소만 정렬 해주는 좁은 범위의 정렬에 집중합니다. 이 접근법은 간단하지만 단 하나의 요소를 정렬하기 위해 너무 많이 교환하는 낭비가 발생할 수도 있있습니다.

### 정렬된 배열

- 버블 정렬은 수행 한 번 만에 모든 원소가 정렬되는 것을 보장하지 않습니다. 그러면 몇 번의 시도를 해줘야 할까요? 예를 들어 6,5,4,3,2,1과 같이 거꾸로 정렬된 경우 다섯 번 시도해야 합니다. 즉 n개의 요소를 정렬해 주기 위해서는 n-1번 실행해주어야 합니다. 최악의 상황인 경우 최대한의 횟수를 실행해줘야 하므로 경제적이지 않습니다.

## topic5 자료 중 가장 작은 것을 찾아 순서대로 정렬하는 방법은 무엇일까요?

### 선택 정렬

- 보통 배열이 정렬되어 있으면 정렬되지 않은 배열보다 더 쉽게 탑색할 수 있습니다. 정렬을 위한알고리즘 중 선택정렬을 배열 안의 자료중 가ㅏ자장 작은 수(혹은 가장 큰수)를 찾아 첫 번째 위치(혹은 가장 마지막 위치)의 수와 교환재는 방식의 정렬입니다.

### 정렬된 배열

- 버블 정렬과는 다르게 몇 번의 교환을 해주었는지 횟수를 셀 필요가 없습니다. 하지만 이 과정은 우리가 해야 할 비교 횟수보다 훨씬 더 많은 비교가 필요하므로 비용이 많이 듭니다. 원래 배열의 순서와 상관없이, 선택 정렬로 정렬되는 배열은 n-1번의 교환이 필요합니다. n-1번의 교환은 확실히 버블 정렬의 교환 횟수보다는 적습니다. 그러나 한 번의 교환이 일어나기 위해서는 정렬되지 않은 수의 모든 비교가 이루어져야 하므로, n제곱번의 비교가 이루어 집니다. 선택 정렬은 최선의 경우에도 최악의 경우에도 최악의 경웨서 수행하는 횟수만큼 비교와 교환을 해주어야 합니다.

## topic6 정렬된 부분, 정렬되지 않은 부분 나누어 정렬하는 방법은 무엇일까요?

### 삽입 정렬

- 자료를 정렬하는 또 다른 알고리즘 중 하나인데, 자료를 여러 번 비교하거나 교환할 필요가 없는 방법이 있습니다. 삽입정렬은 자료가 정렬된 부분과 정렬되지 않은 부분으로 나누어집니다. 정렬되지 않은 부분의 자료가 정렬된 부분의 자리로 삽입되는 형태의 정렬 방법입니다.

### 정렬된 배열

- 삽입 정렬은 특정 실행 단계에서, 어떤 원소가 정렬된 배열 내에 자리를 찾았다고 해서 그것이 최종적이 제자리라는 보장은 없습니다. 다음 단계가 진행되면서 다른 자료에 의해 위치가 바뀔 수 있기 때문입니다. 따라서 삽입 정렬은 자료의 양이 적을 때 성능이 우수하며 자료 대부분이 이미 정렬이 되어있는 경우 효율적입니다. 삽입정렬은 이미 정렬된 자료에 새로운 자료를 삽입해야 하는 경우가 발생하면, 정렬된 자료들이 자리를 이동해야 하므로 안정성이 낮습니다.

## topic7 정렬 알고리즘의 효율성을 높이기 위해서는 무엇을 고려해야 할까요?

### 시간 복잡도

- 시간 복잡도란 알고리즘을 수행할 때 걸리는 시간을 기준으로 효율성을 분석하는 것입니다. 시간의 효율성이란 결국 알고이즘에서 비교와 교환등이 일어날 때 연산자의 처리 횟수가 적다는 의미이며, 연산자의 처리 횟수가 적다는 건 시간의 복잡도가 낮다는 의입니다. 따라서 시간 복잡도가 낮을수록, 연산자의 사용 횟수가 적을수로 효율성이 높은 알고리즘이 됩니다.

### Big-O 표기법

- Big-O 표기법은 컴퓨터 과학에서 "대략"을 나타내는 공식적인 개념으로 최악의 경우에 대한 시간 복잡도를 나타내는 표현입니다.

- 선형 탐색은 비교적 간단한데 찾는 값이 배열의 맨 끝에 있는 최악의 상황의 경우 이 값을 찾는데 n번의 단계를 거치면 됩니다. 이 개념은 O(n)으로 나타납니다.

- 버블 정렬에서는 인접해 있는 자료와 쌍을 이루어 비교하기 때문에, n개의 자료를 갖는 배열은 n-1쌍을 비교합니다. n개의 자료가 있을 때 n-1번 비교해주면, n번째의 자료가 정렬되어있습니다. 그 이후로 n-1개의 자료를 다시 비교하게 됩니다. 전체 비교 횟수는(n-1) +(n-2) + .... +1은 n(n-1)/2이며 n제곱/2 - n/2로 나타낼 수 있습니다. 시간 복잡도는 가장 중요한(가장 지수가 큰) 부분만 남기고, 계수를 삭제합니다. 따라서 만약 n제곱/2 - n/2의 가장 중요한 부분은 n제곱/2이 되며 이것은 (1/2)n2입니다. 계수를 제외하면 n2이 남고 O(n제곱)으로 표현합니다.

- 선택 정렬은 가장 작은 값(혹은 가장 큰 값)을 찾아 제 자리를 찾아줍니다. n개의 자료가 있다면 첫 번째 자료와 나머지 n-1개의 자료 중 가장 작은 값의 자리를 교환해주어야 합니다. n-1개의 자료 중에서 가장 작은 값을 찾기 위해서는 n-1번의 비교가 필요합니다. 즉 비교 횟수는 버블 정렬과 마찬가지로 (n-1) + (n-2) + ..... + 1이며, 시간복잡도는 O(n제곱)으로 표현합니다.

### Big Ω 표기법

- Big-O와 비슷한 Big Ω 표기법이 있는데 Big Ω는 최선의 경우를 나타냅니다.

- 선형 탐색에서 최선의 경우는 배열의 처음에 찾고자 하는 값이 있는 상황입니다. 이는 배열의 크기와 상관없이 Ω(1)이라고 나타냅니다. 버블 정렬에서 최선의 경우(이미 정렬된 배열)를 생각해조면 버블 정렬은 교환이 이루어지지 않더라도 배열이 정렬된 사실을 모르기 때문에 여전히 n-1번의 비교를 해줘야합니다. 그래서 최선의 경우는 Ω(n)로 표기합니다.

- 선택 정렬 역시 배열이 정렬되었다는 것을 알 수 없어, 최소값을 계속 찾아주어야 하므로 Ω(n제곱)로 표기합니다.

- 삽입 정렬은 정렬되지 않은 부분에서 정렬된 부분으로 옮겨갈 때, 정렬된 부준의 가장 큰 수와 비교하기만 하면 되기 때문에 Ω(n)로 표기합니다.

## topic8 많은 자료를 분해하고 다시 합쳐 정렬하는 것을 무엇이라고 할까요?

### 합병 정렬

- 지난 단원에서 다양한 정렬 방법에 대해서 배웠습니다. 하지만 우리가 아직 공부하지 않은 대표적인 정렬 방법이 하나 더 있습니다. 전화번호부의 분할 정복 탐색처럼 데이터를 반으로 나누어간다는 것과 공통점이 있는 방법인 합병 정렬(병합 정렬)이 있습니다. 합병 정렬은 원소가 한 개가 될 때까지 계속해서 반으로 나누다가 다시 합쳐나가며 정렬을 하는 방식입니다. 그리고 이 과정은 재귀적으로 구현되기 때문에 나중에 재귀를 학습하면 더 이해하기 쉽습니다.

### 실행

- 합병 정렬은 배열의 원소들이 반으로 나누어지는 과정과 정렬된 후 합쳐지는 과정으로 나누어져 있습니다. 우리가 만약 3,5,2,6,4,1이라는 배열을 가지고 합병정렬을 이용하여 정렬해야 한다면 의사코드로 작성할 수 있을 것입니다.

### 정렬된 배열

- 분할 정복은 모든 데이터를 다 보는 것이 아니라 절반을 그리고 그 절반을 보는 방식으로 진행되어 탐색 시간이 굉장히 짧았던 것을 기억하시나요? 합병 정렬 역시 반을 나눈다는 개념이 사용되기 때문에 시간이 적게 들 것이라고 유추할 수 있습니다.

- 만약 8개의 원소가 있다면 3번 나누어질 것입니다. 따라서 n개의 원소가 있을 때 완전히 다 나누어지기까지 호출되는 함수의 개수는 log n개라는 것을 알 수 있습니다. 그리고 합병 정렬은 병합하는 알고리즘을 포함합니다. 합쳐지는 과정에서 각 원소들의 크기를 비교하기 때문에 n번의 비교 과정이 있습니다. 즉 한번 나누어질 때마다 n번의 비교 횟수가 추가되는 것입니다. 따라서 합병 정렬의 시간 복잡도는 O(n log n)입니다.

## topic9 정렬된 데이터에서 원하는 값 쉽고 빠르게 찾는 방법은 무엇일까요?

### 이진 탐색

- 주어진 배열을 탐색하는데 사용할 수 있는 다양한 알고리즘이 있습니다. 그 중 하나는 선형 탐색이라는 것인데 이것은 시간이 다소 오래 걸릴 수 있습니다. 만약 여러분이 찾고자 하는 원소가 배열의 끝에 있다고 가정해봅시다. 선형 알고리즘을 사용하면 찾고자 하는 원소를 찾기 위해 배열 전채를 탐색해야 합니다. 선형 탐샥보다 더 빠른 알고리즘으로 이진 탐색이 있습니다. 이진 탐색은 자료를 절반으로 나눈 후 찾는 값이 어는 쪽에 있는지 파악해 탐색의 범위를 반으로 줄여나가는 탐색 알고리즘입니다.

### 효율성과 비효율성

- 배열을 정렬하는 데는 버블 정렬,삽입 정렬, 선택 정렬 등 다양한 방법이 있습니다. 이 정렬 방법은 사신 이진 탐색을 구현하는데 우용합니다. 이진 탐색의 기본은 정렬된 배열을 만들 수 있다는데 가정을 두고 있습니다.

### 이진 탐색 vs 선형 탐색

- 우리가 어떤 부분을 좋게 만들면 반드시 다른 부분에서 비용이 발생한다는 것은 컴퓨터 과학에서는 일반적인 사실입니다. 일반적으로 선형탐색보다 탐색 속도가 짧지만, 배열을 정리하는 시간이 추가됩니다. 그렇기 때문에 선형적으로 배열을 탑색하는 것이 배열을 정렬한 후 이진 탐색을 사용하는 것보다 빠르게 보이고도 하고, 사실 어떤 상황에서는 이것이 사실이기도 합니다.

- 하지만 배열을 여러 번 탐색할 계획하고 있다면 이진 탐색이 유용하게 사용됩니다. 찾고자 하는 값이 배열에 없는 경우 선형 탐색은 배열의 길이가 얼마든 상관없이 배열 전체를 흝어보아야 배열 안에 찾고자 하는 값이 없다는 것을 알 수 있습니다. 이에 반해 이진 탐색에서는 더 효율적으로 사용할 수 있습니다. 의사 코드를 수행해보면, 찾고자 하는 값이 최소값보다 작거나 최대값보다 크다면 해당 원소가 배열 안에 없다는 것을 알 수 있습니다.
