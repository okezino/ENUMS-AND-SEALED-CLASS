# ENUMS AND SEALED CLASS
> 
>Differences
>
> >sealed class is  Flexible to handle different states of subclass,Enum classs is  not flexible
>
> Similairty
>
>>Restricted number of Hierachies{subclass can't be built outside the class} 
>



## Enum Class

Enum class is a splecial class that takes in a set of Uppercase constants that can act as object of the class, each Constant is seperated by a comma and has a default property of (name and ordinal(position of the constant in the enum class)) 

```kotlin
enum class Sex{
     MALE,
     FEMALE,
     TRANSGENDER
}
```
An enum class can take a constructor() of properties, this must be instantiated in all the various values in the enum class, else we have an error. a new value can not be created outside the class..we can iteterate through an enum class like an Array using a Loop



## Sealed class

This is a special class that allows diffrent form of its Subclass and Objects within its class, Just like  Abstract class, we can freely create subclasses with different constructor parameters within the parent class.

```kotlin

sealed class footballTeam {

data class Manager(var purchaseFund:String = "ffcfcdxd") : FootballTeam()

class Keepers(var glooves: Int = 8, var longsleevejersey: Boolean = true )

object Stricker : footballTeam()

}

```

and like enum class, a sealed class cannot be extended outside its class.

# Conclusion

A sealed class takes the flexible nature of the subclass form of an Abstract class and the restricted nature of hierachies an enum class, making it a prefered class to use.








