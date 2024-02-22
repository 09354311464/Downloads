class Vehicle:
    def __init__(self,name=""):
        self.name=name
    def setWeight(self,weight):
      if(weight>0):
        self.weight=weight
    def setSpeed(self,speed):
      if(speed>0):
        self.speed=speed
    def setFuel(self,fuel):
      self.fuel=fuel
    def getWeight(self):
      return self.weight
    def getSpeed(self):
      return self.speed
    def getFuel(self):
      return self.fuel
        
class Car(Vehicle):
    id=1
    def __init__(self,weightCar,speedCar,fuelCar,Tire):
        Vehicle.__init__(self,weightCar,speedCar,fuelCar)
        id=id+1
        self.Tire=Tire
class Plane(Vehicle):
    def __init__(self,weightPlane,speedPlane,fuelPlane,MaximumHeight):
        Vehicle.__init__(self,weightPlane,speedPlane,fuelPlane)
        self.MaxiumumHeight=MaximumHeight

vasileNaghlie=Vehicle("tank")

vasileNaghlie.setWeight(100)

w=vasileNaghlie.getWeight()

print(w)

w=w+100

vasileNaghlie.setWeight(w)

print(vasileNaghlie.getWeight())