import tkinter as tk
from PIL import Image, ImageTk


root = tk.Tk()
root.geometry("1600x850")  # Set window size

#GAME LOGIC
import random #IMPORT RANDOM TO SELECT ITEM RANDOMLY BY OS 
from colorama import Fore, init

# Load and resize the image to fit the window
bg_image = Image.open("bg.jpg.jpg")
bg_resized = bg_image.resize((1600, 850))
bg_photo = ImageTk.PhotoImage(bg_resized)


# Display the image as background
bg_label = tk.Label(root, image=bg_photo)
bg_label.place(x=0, y=0, relwidth=1, relheight=1)
ee=""
gue=""
gg=""
i=0
def yee():
     def color(guess,c):  #FOR CHANGE THE TEXT COLOR 
       from colorama import Fore, Style, init
       global combine
       button2.delete("1.0", tk.END) #RESET THE 3RD BOX 
       button2.tag_configure("red", foreground="red")
       button2.tag_configure("green", foreground="green")
       for j in range(len(guess)):
         if(guess[j] in c):
                 button2.insert("end",guess[j], "green") #ADD THE LETTER ON 3RD BOX WITH COLOR GREEN
         else:
                 button2.insert("end",guess[j], "red")
     
                   
     
   
     d=3#NUMBER OF ATTEMPTS 
     def selection(item,d,name):#THIS FUNCTION IS USED TO CREATE CHECK USER INPUT AND SHWING OUTPUT
            global ee
            global gue
            global gg
            select=random.randint(0,len(item)-1)#IT SELECT THE RANDOM INDEX FROM THE LIST ITEM
            c=item[select]#WITH THE HELP OF THE INDEX WE SELECT THE NAME OF ANY BIRD
            print(c)#OUTPUT OF LETTER
            print(F"{Fore.CYAN}THIS IS THE NAME OF {name} WHICH CONTAIN {len(c)} LETTERS")#THIS IS BASICALLY USED TO PRINT THE MESSAGE
            ee=F"THIS IS THE NAME OF {name} WHICH CONTAIN {len(c)} LETTERS"
            entry1.config(text=ee)
          
            def check():
              global i 
              if(i<d):  
                def answer():
                 global gg
                 gue=entry.get().upper()#TAKING INPUT FROM USER IN CAPITAL LETTER TO COMPARE WITH OUR SELECT ITEM NAME  
                 return gue
                guess=answer()
                if(guess==c):
               # import shared as s
                    print(color(guess,c))
                    entry2.delete("1.0", tk.END)
                    gg=f"YEE HOO YOU GIVE RIGHT ANSWER 😎  ✌  ✌"
                    entry2.config(fg="green",bg="black")
                    entry2.insert(tk.END, gg)
                    return 0
   
                else:
                   print(color(guess,c))
                   gg=f"OOPS!YOUR ANSWER IS WRONG. NOW YOU HAVE ONLY {d-i-1} ATTEMPT 🤡 🤡"
                   entry2.delete("1.0", tk.END)
                   entry2.config(fg="red",bg="black")
                   entry2.insert(tk.END,gg)
                   i=i+1
                 
              else:
                 gg=f"RIGHT ANSWER 😊  😎: ",c
                 entry2.delete("1.0", tk.END)
                 entry2.config(fg="yellow",bg="black")
                 entry2.insert(tk.END,gg)
                 i=0
                 replay= tk.Button(root,text="SWITCH",font=("Arial",30),bg="black",fg="white",command=yee)#REPLAY BUTTON 
                 replay.place(x=1110, y=445)
            button1 = tk.Button(root, text="SUBMIT",command=check,font=("Arial",32),bg="Light blue")
            button1.place(x=1100, y=335)  
# import shared as s #IMPORT SHARED as S THIS IS USED FOR COMBINING THE CODE WHICH IS WRITTEN IN ANOTHER PAGE 
     def birds():
         item = [
    "PEACOCK", "SPARROW", "PIGEON", "CROW", "PARROT", "EAGLE", "OWL", "DUCK", "KINGFISHER", "FLAMINGO",
    "MYNA", "KOEL", "DOVE", "KITE", "BLACK DRONGO", "INDIAN ROBIN", "WHITE-BREASTED KINGFISHER",
    "JUNGLE BABBLER", "BRAHMINY KITE", "INDIAN ROLLER", "HOOPOE", "GREY FRANCOLIN", "COMMON MYNA",
    "ORIENTAL MAGPIE ROBIN", "ROSE-RINGED PARAKEET", "PURPLE SUNBIRD", "BULBUL", "ASIAN KOEL", 
    "HOUSE CROW", "CATTLE EGRET", "PIED BUSHCHAT", "INDIAN POND HERON", "GREEN BEE-EATER",
    "INDIAN SILVERBILL", "RED-VENTED BULBUL", "INDIAN ORIOLE", "COMMON IORA", "GREAT EGRET", 
    "BLACK KITE", "SPOTTED OWLET", "RED-WATTLED LAPWING", "INDIAN PEAHEN", "PIED KINGFISHER",
    "GREEN PIGEON", "RUFOUS TREEPIE", "INDIAN GREY HORNBILL", "WHITE-THROATED KINGFISHER",
    "ASHY PRINIA", "SPOTTED DOVE", "INDIAN BUSH LARK"
   ]
         name="BIRD"
         selection(item,d,name)#CALL SELECTION FUNCTION
    



#ANIMALS LIST
     def animal():
    # import WORD_GAME as w#THIS IS USED FOR COMBINING THE CODE WHICH IS WRITTEN IN ANOTHER PAGE 
         item = [
    "DOG", "CAT", "COW", "HORSE", "CHICKEN", "SHEEP", "GOAT", "PIG", "LION", "TIGER",
    "ELEPHANT", "MONKEY", "BEAR", "DEER", "SNAKE", "RABBIT", "SQUIRREL", "FISH", "DOLPHIN", "WHALE",
    "SHARK", "CROCODILE", "ALLIGATOR", "ZEBRA", "GIRAFFE", "CHEETAH", "LEOPARD", "FOX", "WOLF",
    "KANGAROO", "PANDA", "KOALA", "RHINOCEROS", "HIPPOPOTAMUS", "BAT", "PEACOCK", "PARROT", "PIGEON",
    "BUTTERFLY", "SPARROW", "OWL", "EAGLE", "HAWK", "FALCON", "TURTLE", "FROG", "TOAD", "IGUANA",
    "LIZARD", "CATERPILLAR", "SPIDER", "SCORPION", "ANT", "BEE", "MOSQUITO", "FLY", "CRAB", "LOBSTER",
    "OCTOPUS", "JELLYFISH", "STARFISH", "CHIMPANZEE", "GORILLA", "OTTER", "RACCOON", "SKUNK", "HYENA",
    "ORANGUTAN", "MOOSE", "BISON", "BUFFALO", "CAMEL", "WALRUS", "SEAL", "FERRET", "MEERKAT", "HEDGEHOG",
    "BADGER", "LYNX", "BOBCAT", "WOLVERINE", "HONEY BADGER", "MANATEE", "DINGO", "ANTELLOPE", "GAZELLE",
    "IBEX", "MULE", "PECCARY", "LEMUR", "KUDU", "ELAND", "OKAPI", "PORCUPINE", "CARIBOU", "PRAIRIE DOG",
    "ARMADILLO", "PANGOLIN", "TAPIR", "VICUNA", "SPRINGBOK", "SLOTH", "CHINCHILLA", "BONGO", "AGOUTI"
   ]
         name="ANIMAL"
         selection(item,d,name)

#FLOWERS LIST
     def flower():
    # import WORD_GAME as w#THIS IS USED FOR COMBINING THE CODE WHICH IS WRITTEN IN ANOTHER PAGE 
         item = [
    "ROSE", "TULIP", "LILY", "DAFFODIL", "ORCHID", "JASMINE", "SUNFLOWER", "DAISY", "MARIGOLD", "CARNATION",
    "LOTUS", "CHERRY BLOSSOM", "LAVENDER", "VIOLET", "HIBISCUS", "CROCUS", "PEONY", "CAMILIA", "GERANIUM",
    "AZALEA", "IRIS", "CAMPANULA", "FREESIA", "HEDGES", "PLUMERIA", "GERBERA", "PANSY", "ZINNIA", "PETUNIA",
    "BEGONIA", "IMPATIENS", "SNAPDRAGON", "HELLEBORE", "AMARYLLIS", "GARDENIA", "HOLLYHOCK", "NARCISSUS",
    "ALSTROEMERIA", "SCABIOSA", "STOCK", "YARROW", "TIGER LILY", "MARANTA", "WISTERIA", "FUCHSIA", "BLOODROOT",
    "CHRISTMAS CACTUS", "POTTED PRIMROSE", "CALLA LILY", "COLUMBINE", "ASTER", "MORNING GLORY", "PETALONIA"
   ]
         name="FLOWER"
         selection(item,d,name)

#BODY ORGANS NAME
     def organs_name():
    # import WORD_GAME as w#THIS IS USED FOR COMBINING THE CODE WHICH IS WRITTEN IN ANOTHER PAGE 
         item = [
    "HEART", "BRAIN", "LIVER", "KIDNEY", "LUNGS", "STOMACH", "INTESTINE", "BLADDER", "SKIN", "SPLEEN",
    "PANCREAS", "EYES", "EARS", "NOSE", "MOUTH", "TEETH", "TONGUE", "BONES", "MUSCLES", "BLOOD VESSELS",
    "NERVES", "THYMUS", "ADRENAL GLANDS", "THYROID", "PARATHYROID GLANDS", "PITUITARY GLAND", "PINEAL GLAND",
    "PROSTATE", "OVARIES", "TESTES", "LARYNX", "PHARYNX", "TRACHEA", "ESOPHAGUS", "COLON", "RECTUM", "ANUS",
    "LARGE INTESTINE", "SMALL INTESTINE", "APPENDIX", "CEREBELLUM", "CEREBRUM", "CORNEA", "RETINA", "OPTIC NERVE",
    "CORONARY ARTERIES", "LYMPH NODES", "LYMPHATIC VESSELS", "VAGINA", "CERVIX", "URETHRA"
   ]
         name="BODY ORGAN"
         selection(item,d,name)


#CITY NAME
     def city():
    # import WORD_GAME as w#THIS IS USED FOR COMBINING THE CODE WHICH IS WRITTEN IN ANOTHER PAGE 
         item = [
    "MUMBAI", "DELHI", "KOLKATA", "BENGALURU", "CHENNAI", "HYDERABAD", "PUNE", "AHMEDABAD", "Kochi", "LUCKNOW",
    "JAIPUR", "SURAT", "PATNA", "INDORE", "CHANDIGARH", "BHOPAL", "VADODARA", "VISAKHAPATNAM", "GOA", "RANCHI",
    "MYSURU", "THANE", "KANPUR", "AGRA", "VARANASI", "NAGPUR", "BHUJ", "SHIMLA", "DEHRA DUN", "GURUGRAM",
    "NOIDA", "FARIDABAD", "IMPHAL", "DISPUR", "PORT BLAIR", "GAYA", "JAMMU", "LEH", "MANALI", "SRINAGAR",
    "JAISALMER", "JODHPUR", "BIKANER", "UDAIPUR", "RISHIKESH", "BARNALA", "LUDHIANA", "RAIPUR", "KHARAGPUR", 
    "MIRZAPUR", "JABALPUR", "TIRUNELVELI", "NASHIK", "BELAGAVI", "SHIRDI"
   ]
         name="CITY"
         selection(item,d,name)


#CARS NAME
     def car():
    # import WORD_GAME as w#THIS IS USED FOR COMBINING THE CODE WHICH IS WRITTEN IN ANOTHER PAGE 
         item = [
    "TOYOTA COROLLA", "HONDA CIVIC", "HYUNDAI SANTRO", "MARUTI SUZUKI SWIFT", "TATA NEXON", "HONDA CITY",
    "TOYOTA CAMRY", "MARUTI SUZUKI BALENO", "FORD FIESTA", "RENAULT KWID", "NISSAN MICRA", "MAHINDRA XUV500",
    "HYUNDAI CRETA", "TOYOTA INNOVA", "MARUTI SUZUKI DZIRE", "HYUNDAI I20", "TOYOTA FORTUNER", "MAHINDRA THAR",
    "MARUTI SUZUKI ALTO", "KIA Seltos", "TATA TIAGO", "HONDA JAZZ", "FORD ECOSPORT", "SKODA RAPID", "VOLKSWAGEN POLO",
    "TATA HARIER", "RENAULT DUSTER", "SUZUKI VITARA", "HYUNDAI VENUE", "HONDA WR-V", "MARUTI SUZUKI CELERIO",
    "MITSUBISHI OUTLANDER", "CHEVROLET SPARK", "FIAT PUNTO", "NISSAN SUNNY", "TOYOTA YARIS", "HYUNDAI TUCSON",
    "KIA SONET", "MARUTI SUZUKI ERTIGA", "TATA ALTROZ", "MAHINDRA SCORPIO", "NISSAN TERRANO", "HONDA ACCORD", "BMW 3 SERIES",
    "MERCEDES-BENZ E-CLASS", "AUDI A4", "SKODA OCTAVIA", "TOYOTA LAND CRUISER", "SUZUKI WAGON R", "VOLKSWAGEN TIGUAN",
    "HONDA CR-V", "HYUNDAI I10"
   ]
         name="CAR"
         selection(item,d,name)


#GADGETS NAME 
     def gadget():
    # import WORD_GAME as w#THIS IS USED FOR COMBINING THE CODE WHICH IS WRITTEN IN ANOTHER PAGE 
         item = [
    "SMARTPHONE", "LAPTOP", "TABLET", "SMARTWATCH", "WIRELESS EARPHONES", "EARBUDS", "POWER BANK", 
    "FITNESS TRACKER", "DIGITAL CAMERA", "DRONE", "SMART TV", "MICROWAVE OVEN", "AIR PURIFIER", "KITCHEN BLENDER",
    "GAMING CONSOLE", "PRINTER", "HEADPHONES", "SMART SPEAKER", "E-READER", "GAMING MOUSE", "GAMING KEYBOARD",
    "VIRTUAL REALITY HEADSET", "ELECTRIC TOOTHBRUSH", "ROBOT VACUUM", "SMART LIGHTBULB", "BLUETOOTH SPEAKER", 
    "SMART PLUG", "MICROPHONE", "PROJECTOR", "EXTERNAL HARD DRIVE", "USB FLASH DRIVE", "ACTION CAMERA", 
    "WIFI ROUTER", "RICE COOKER", "SLOW COOKER", "COFFEE MACHINE", "HAIR DRYER", "SMART THERMOSTAT", "SMART LOCK",
    "DRY IRON", "STEAM IRON", "RECHARGEABLE FAN", "COOLING PAD", "DESK LAMP", "VIDEO DOORBELL", "LAPTOP COOLER",
    "ROBOTIC TOY", "CAMERA GIMBAL", "BLUETOOTH RECEIVER", "SOLAR POWER BANK", "INDOOR GARDEN KIT", "FOOD DEHYDRATOR",
    "WIRELESS CHARGER", "ACTION CAMERA", "SMARTGLASSES", "PORTABLE AIR CONDITIONER", "SECURITY CAMERA", "GUITAR TUNER"
   ]
         name="GADGET"
         selection(item,d,name)


#NORMAL WORDS
     def word():
    # import WORD_GAME as w#THIS IS USED FOR COMBINING THE CODE WHICH IS WRITTEN IN ANOTHER PAGE 
         item = [
    "WAKE UP", "BRUSH", "SHOWER", "BREAKFAST", "LUNCH", "DINNER", "WORK", "STUDY", "READ", "WRITE",
    "EXERCISE", "RELAX", "MEETING", "CALL", "TEXT", "WALK", "CLEAN", "COOK", "SHOP", "LAUNDRY", "TIDY",
    "SLEEP", "WAKE", "WATCH TV", "WATCH MOVIE", "LISTEN", "EAT", "DRINK", "CHAT", "GREET", "HUG", "SMILE",
    "LAUGH", "SING", "DANCE", "JOG", "GARDEN", "TIDY UP", "ORGANIZE", "VISIT", "HELP", "PLAN", "MEDITATE",
    "RELAX", "STRETCH", "GIVE", "RECEIVE", "THANK", "APOLOGIZE", "MEET", "LEAVE", "ARRIVE", "CLOSE", "OPEN",
    "DECIDE", "CHOOSE", "SCHEDULE", "SHOPPING", "BUY", "SELL", "PAY", "RECEIVE", "WORKOUT", "REST", "TALK",
    "SIT", "STAND", "WAIT", "ANSWER", "ASK", "FOLLOW", "LEARN", "REMIND", "FORGET", "ACCEPT", "REFUSE", "GO"
   ]
         name="WORD"
         selection(item,d,name)


     items =[birds,animal,flower,organs_name,gadget,city,car,word] #FUNCTION CREATED UNDER ITEMS_NAME FILE
     select=items[random.randint(0,len(items)-1)]()#WITH THE HELP OF THIS IT AUTOMATICALLY SELECT ANY FUN() FROM ITEMS LIST
   




# Entry for user input
entry = tk.Entry(root,font=("Arial",55),bg="black",fg="white") #2ND DABBA
entry.place(x=270,y=335)

entry1 = tk.Button(root,text=ee,font=("Arial",24),bg="black",fg="white",width=55, height=2)#1ST DABBA
entry1.place(x=260,y=200)

button2 = tk.Text(root,font=("Arial",24),bg="black",width=57, height=2)#3RD DABBA
button2.place(x=270,y=447)

entry2 = tk.Text(root,font=("Arial", 22),width=64, height=2, bg="#ddd0c8")#LAST DABBA
entry2.place(x=270,y=560)

replay= tk.Button(root,text="SWITCH",font=("Arial",30),bg="black",fg="white",command=yee)#REPLAY BUTTON 
replay.place(x=1110, y=445)

yee()
root.mainloop()
