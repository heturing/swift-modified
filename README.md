This is the solution to a programming task.

To build this version of swift, please follow the instruction in file <a href="https://github.com/apple/swift/blob/master/README.md" target="_blank">README.md</a>

As a demo, create a swift source file called `test.swift` with the following content:

    class Person {
      var name = ""
      var age = 0
      func call(name: String, phone: String, message: String, count: Int) {
        
      }

      func reset() {
        name = ""
        age = 0
      }
    }

Then, execute:
    
    your-path-to-swiftc test.swift 
    
And your should see a warning message shows up.

An example:

    $ ../swift-source/build/Ninja-RelWithDebInfoAssert/swift-linux-x86_64/bin/swiftc test.swift
 
      test.swift:4:12: warning: a function with more than three parameters
      func call(name: String, phone: String, message: String, count: Int) {
               ^
    
