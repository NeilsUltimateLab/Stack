# Stack
Swift stack

This class is the Represent the Array as Stack for Push Pop Operations


    import Foundation

    public struct Stack<T> {

      fileprivate var array = [T]()
    
      public var isEmpty: Bool {
          return array.isEmpty
      }
    
      public var count: Int {
          return array.count
      }
    
      public mutating func push(_ element: T) {
          array.append(element)
      }
    
      public mutating func pop() -> T? {
          return array.popLast()
      }
    
      public func peek() -> T? {
          return array.last
      }
    
      public mutating func trash() {
          array.removaAll()
      }
    
    }
