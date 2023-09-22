void main() {
  List<String> names = ['ali', 'abdullah', 'hamza', 'ahmed', 'omais'];

  for (String name in names) {
    print(name);
  }
}

void main (){
  List<String> days = [];
  
    
  days.add('Monday');
  days.add('tuesday');
  days.add('Wednesday');
  days.add('Thursday');
  days.add('Friday');
  days.add('Saturday');
  days.add('Sunday');

  for (String day in days){
    print (day);
  
  }
  
}

void main() {
  List<String> days = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday'];

 
  while (days.isNotEmpty) {
    String removedDay = days.removeLast();
    print('Removed: $removedDay');
  }
}




void main() {
  List<int> numbers = [18, 5, 2, 3, 1, 15, 14];

  int smallest = numbers[0];
  int greatest = numbers[0];

  for (int number in numbers) {
    if (number < smallest) {
      smallest = number;
    }
    if (number > greatest) {
      greatest = number;
    }
  }

  print('Smallest number: $smallest');
  print('Greatest number: $greatest');
}


void main() {
  List<String> usersEligibility = ['John', 'Alice', 'eligible', 'Mike', 'Sarah', 'Tom'];

  usersEligibility.removeWhere((element) => element == 'eligible');

  print(usersEligibility);
}


void main() {
  List<int> numbers = [10, 5, 8, 20, 3, 15, 7];

  int maximum = numbers.reduce((currentMax, next) => currentMax > next ? currentMax : next);

  print('Maximum value: $maximum');
}



List<String> removeDuplicates(List<String> inputList) {
  Set<String> uniqueSet = Set<String>();
  List<String> result = [];

  for (String element in inputList) {
    if (!uniqueSet.contains(element)) {
     
    }
  }

  return result;
}

void main() {
  List<String> originalList = ['apple', 'banana', 'apple', 'cherry', 'banana', 'date'];
  List<String> withoutDuplicates = removeDuplicates(originalList);

  print('Original List: $originalList');
  print('List Without Duplicates: $withoutDuplicates');
}


List<T> takeFirstN<T>(List<T> originalList, int n) {
  if (n <= 0) {
    return [];
  }
  if (n >= originalList.length) {
    return List.from(originalList);
  }
  return originalList.sublist(0, n);
}

void main() {
  List<int> originalList = [1, 2, 3, 4, 5, 6, 7];
  int n = 3;

  List<int> firstNElements = takeFirstN(originalList, n);

  print('Original List: $originalList');
  print('First $n Elements: $firstNElements');
}


void main() {
  List<String> originalList = ['apple', 'banana', 'cherry', 'date', 'fig'];
  
  List<String> reversedList = reverseList(originalList);

  print('Original List: $originalList');
  print('Reversed List: $reversedList');
}



List<int> getUniqueElements(List<int> originalList) {
  List<int> uniqueList = [];

  for (int number in originalList) {
    if (!uniqueList.contains(number)) {
      uniqueList.add(number);
    }
  }

  return uniqueList;
}

void main() {
  List<int> originalList = [1, 2, 2, 3, 4, 4, 5];
  
  List<int> uniqueElements = getUniqueElements(originalList);

  print('Original List: $originalList');
  print('Unique Elements List: $uniqueElements');
}


List<int> sortList(List<int> originalList) {
  List<int> sortedList = List.from(originalList);
  sortedList.sort();
  return sortedList;
}

void main() {
  List<int> originalList = [5, 2, 8, 1, 9, 3];
  
  List<int> sortedElements = sortList(originalList);

  print('Original List: $originalList');
  print('Sorted List (Ascending): $sortedElements');
}


List<int> filterPositiveNumbers(List<int> originalList) {
  return originalList.where((number) => number > 0).toList();
}

void main() {
  List<int> originalList = [5, -2, 8, -1, 9, -3];
  
  List<int> positiveNumbers = filterPositiveNumbers(originalList);

  print('Original List: $originalList');
  print('Positive Numbers: $positiveNumbers');
}



List<int> filterEvenNumbers(List<int> originalList) {
  return originalList.where((number) => number % 2 == 0).toList();
}

void main() {
  List<int> originalList = [5, 2, 8, 1, 9, 6, 3];
  
  List<int> evenNumbers = filterEvenNumbers(originalList);

  print('Original List: $originalList');
  print('Even Numbers: $evenNumbers');
}


void main() {
  
  List<String> list1 = ['apple', 'banana', 'cherry', 'date', 'gava'];
  List<int> list2 = [1, 2, 3, 4, 5, 6, 7];
  List<bool> list3 = [true, false, true, true, false, false];

  
  list1.replaceRange(2, 3, ['grape']);

  
  list2.replaceRange(list2.length - 3, list2.length - 2, [8]);

  
  list3.replaceRange(1, 4, [false, true, true]);

 
  print('List 1: $list1');
  print('List 2: $list2');
  print('List 3: $list3');
}


List<int> squareList(List<int> originalList) {
  return originalList.map((number) => number * number).toList();
}

void main() {
  List<int> originalList = [1, 2, 3, 4, 5];
  
  List<int> squaredList = squareList(originalList);

  print('Original List: $originalList');
  print('Squared List: $squaredList');
}

