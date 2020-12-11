# ENUMS AND SEALED CLASS
> 
>Differences
>
> >Flexible to handle diiferent states of subclass,Enum classs is  not flexible
>
> Similairty
>
>>Restricted number of Hierachies{subclass cant be built outside the class} 
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
An enum class can take a constructor() of properties, this must be instantiated in all the various values in the enum class, else we have a error. a new value ca not be created outside the class..we can iteterate through an enum class like an Arrayusing a Loop



## Sealed class

This is a special class that allows diffrent form of its Subclass and Objects within its class, Just like  Abstract class, we can freely create subclasses with different constructor parameters wiithin the parent class.

```kotlin

sealed class footballTeam {

data class Manager(var purchaseFund:String = "ffcfcdxd") : FootballTeam()

class Keepers(var glooves: Int = 8, var longsleevejersey: Boolean = true )

object Stricker : footballTeam()

}

```

and like enum class, a sealed class cannot be extended outside its class.








