 # Swift-UserDefaults
You love Swift's Codable protocol and use it everywhere, who doesn't! Here is an easy and very light way to store and retrieve -reasonable amount- of Codable objects, in a couple lines of code!



Foobar is a Python library for dealing with word pluralization.

## Installation

Download project , drag and draw file "DefaultsBuilder.swift".


## Usage

```python
Create your Defaults file.

enum Defaults :String ,KKDefaultsBuilder
{
    case isLogin
    case lang
    case id
    case user
}

//================

  guard let islogin : Bool  = Defaults.isLogin.get()  else {
            return
        }
        print(islogin)
        
        Defaults.id.save(12)
        Defaults.lang.save("en")


```

//Retrieve
```python
    guard let user : User  = Defaults.user.get()  else {
            print("nil")
            return
        }
        print("user" , user)

```
//Model To save
```python
struct User : Codable {
    
    let name : String = ""
    let id : Int = 10
}
```
