import UIKit
import Foundation


//  Исходный массив
var array = [6, -2, 8, -3, 0, -7, 1, 10, 15, -9]


// 1 – Заменить в массиве отрицательные числа нулем

for i in 0..<array.count {
    if array[i] < 0 {
        array[i] = 0
    }
}
print("1 - замена отрицательных чисел нулями:", array)


// 2 – Сортировка массива по убыванию(возрастанию)
let sortedArrayMax = array.sorted()
print("2 - сортировка по возрастанию:",sortedArrayMax)

let sortedArrayMin = array.sorted(by: >)
print("2 - сортировка по убыванию:",sortedArrayMin)


// 3 – Найти max(min) элемент в массиве
let maxElement = array.max() ?? 0
print("3 - максимальный элемент:", maxElement)

let minElement = array.min() ?? 0
print("3 - минимальный элемент:", minElement)


// 4 – Найти сумму элементов массива
let sumArray = array.reduce(0, +)
print("4 - сумма элементов:", sumArray)
