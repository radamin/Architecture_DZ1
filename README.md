[U@startuml
interface OOP_HW02_Aquarium.EatingFish {
~ int eatedFishes()
}
class OOP_HW02_Aquarium.Aqarium {
- Water
- List<AquaResidents> aquarium
- Cleaner joe
- Cleaner bob
+ Aqarium addAquaResidents(AquaResidents)
- List<AquaSoundAble> getAquaSoundable()
+ String getAquaSound()
+ List<EatingFish> ateFishes()
+ List<HitingSuperCombo> heroes()
+ HitingSuperCombo getSuperChamp(List<HitingSuperCombo>)
+ EatingFish getMainGuzzler(List<EatingFish>)
+ String toString()
}
abstract class OOP_HW02_Aquarium.Residents.Base.PredatoryFish {
}
interface OOP_HW02_Aquarium.HitingSuperCombo {
~ String hitingSuperCombo()
~ int getComboStrength()
}
class OOP_HW02_Aquarium.Cleaner {
~ String cleanerName
~ String cleanerWeapon
~ String cleanerSuperPunch
+ String hitingSuperCombo()
+ int getComboStrength()
+ String toString()
+ int eatedFishes()
}
class OOP_HW02_Aquarium.Residents.AquaMan {
+ String sound()
+ String toString()
+ int eatedFishes()
}
class OOP_HW02_Aquarium.Water {
+ String sound()
}
class OOP_HW02_Aquarium.Residents.Turtle {
+ String sound()
+ int eatedFishes()
}
class OOP_HW02_Aquarium.Residents.ClownFish {
+ String sound()
}
abstract class OOP_HW02_Aquarium.Residents.Base.Fishes {
+ String sound()
}
abstract class OOP_HW02_Aquarium.Residents.Base.HerbivorousFish {
}
class OOP_HW02_Aquarium.Residents.Piranha {
+ String toString()
+ int eatedFishes()
}
class OOP_HW02_Aquarium.Residents.NinjaTurtle {
- String superPunch
- String beltColor
- String weapon
+ String sound()
+ String toString()
+ String hitingSuperCombo()
+ int getComboStrength()
}
abstract class OOP_HW02_Aquarium.Residents.Base.AquaResidents {
- String type
- String name
+ String toString()
}
abstract class OOP_HW02_Aquarium.Residents.Base.Amphibians {
}
interface OOP_HW02_Aquarium.AquaSoundAble {
~ String sound()
}
class OOP_HW02_Aquarium.Main {
+ {static} void main(String[])
}


OOP_HW02_Aquarium.EatingFish <|.. OOP_HW02_Aquarium.Residents.Base.PredatoryFish
OOP_HW02_Aquarium.Residents.Base.Fishes <|-- OOP_HW02_Aquarium.Residents.Base.PredatoryFish
OOP_HW02_Aquarium.HitingSuperCombo <|.. OOP_HW02_Aquarium.Cleaner
OOP_HW02_Aquarium.EatingFish <|.. OOP_HW02_Aquarium.Cleaner
OOP_HW02_Aquarium.EatingFish <|.. OOP_HW02_Aquarium.Residents.AquaMan
OOP_HW02_Aquarium.Residents.Base.AquaResidents <|-- OOP_HW02_Aquarium.Residents.AquaMan
OOP_HW02_Aquarium.AquaSoundAble <|.. OOP_HW02_Aquarium.Water
OOP_HW02_Aquarium.EatingFish <|.. OOP_HW02_Aquarium.Residents.Turtle
OOP_HW02_Aquarium.Residents.Base.Amphibians <|-- OOP_HW02_Aquarium.Residents.Turtle
OOP_HW02_Aquarium.Residents.Base.HerbivorousFish <|-- OOP_HW02_Aquarium.Residents.ClownFish
OOP_HW02_Aquarium.Residents.Base.AquaResidents <|-- OOP_HW02_Aquarium.Residents.Base.Fishes
OOP_HW02_Aquarium.Residents.Base.Fishes <|-- OOP_HW02_Aquarium.Residents.Base.HerbivorousFish
OOP_HW02_Aquarium.Residents.Base.PredatoryFish <|-- OOP_HW02_Aquarium.Residents.Piranha
OOP_HW02_Aquarium.HitingSuperCombo <|.. OOP_HW02_Aquarium.Residents.NinjaTurtle
OOP_HW02_Aquarium.Residents.Turtle <|-- OOP_HW02_Aquarium.Residents.NinjaTurtle
OOP_HW02_Aquarium.AquaSoundAble <|.. OOP_HW02_Aquarium.Residents.Base.AquaResidents
OOP_HW02_Aquarium.Residents.Base.AquaResidents <|-- OOP_HW02_Aquarium.Residents.Base.Amphibians
@endumlploading OOP_HW02_AquariumUML.puml…]()



