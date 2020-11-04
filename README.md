# thelonapiasotojoker (Θέλω να πιάσω το Τζόκερ)

streamlit web app to create random wheels based on certain rules for 5 out 45 greek Joker Lottery.
Choose the number of wheels you want (10-30) and download them as a csv file.
The rules on which the random selection is based on are explaied below.
The main idea for this app is to create wheels that seem highly probable to win with higher expectancy 
to occur based on the history of the game.

το web app με το οποίο δεν παίζεις Τζόκερ μόνος διαλέγοντας αριθμούς στην τύχη αλλά επιλέγοντας στήλες με "χαρακτηριστικά" τέτοια που η αναμενόμενη στατιστική τους επαλήθευση να είναι μεγαλύτερη από το ποσοστό του συνόλου των στηλών με τα 'χαρακτηριστικά' αυτά.
πχ. στήλες με ένα ή κανένα ζευγάρι συνεχόμενων αριθμών είναι συνολικά 1.154.478 στις 1.221.759 δηλ. το 94,5%, ενώ στο σύνολο των 2291 κληρώσεων που έχουν πραγματοποιηθεί, έχει κληρωθεί στήλη με μέχρι ένα ζευγάρι συνεχόμενων αριθμών 2178 φορές δηλ. 95,1%. Αυτό μας λέει ότι το "χαρακτηριστικό" αυτό έχει αναμενόμενη στατιστική επαλήθευση μεγαλύτερη από όσο θα ΄πρεπε με βάση το πλήθος των στηλών που υπάρχουν με το 'χαρακτηριστικό' αυτό άρα είναι πολύ καλό χαρακτηριστικό και δεν χρειάζεται να παίξουμε στήλη που να έχει 2 ζευγάρια συνεχόμενων αριθμών.

Ενα πολύ καλό χαρακτηριστικό που κόβει πάρα πολλές στήλες είναι να παίζουμε στήλες που δεν έχουν 4 κοινούς αριθμούς με καμιά από τις προηγούμενες στήλες.  Αυτό μας δίνει μόνο 819.502 στις 1.221.759 και εννοείται ότι ο όρος καλυτερεύει κόβοντας κι άλλες στήλες όσο γίνονται κληρώσεις. Το ποσοστό των στηλών είναι 67,1% ενώ η στατιστική επαλήθευση φθάνει το 81,7% αφού 1871 στις 2291 κληρώσεις έχουμε τέτοια στήλη.

Αλλο ένα παράδειγμα τέτοιου χαρακτηριστικού είναι, το πλήθος των διαφορών μεταξύ οποιωνδήποτε από τους 5 αριθμούς να είναι 5 ή 10, να είναι μέχρι μια. Προκύπτει ότι υπάρχουν 1049799 τέτοιες στήλες ήτοι 85,9% και έχει στατιστική επαλήθευση 1871 φορές στις 2291 δηλ. 87,1%.

Αν βάλουμε και τους 3 όρους (χαρακτηριστικά) τότε έχουμε 662904/1221759 δηλ. 54,3% και ο συνδυασμός τους επαληθεύεται μέχρι σήμερα 1555/2291 φορές δηλ. 67,9% Αυτό σημαίνει 25% μεγαλύτερη στατιστικη επαλήθευση.
ΑΝ προσθέσουμε σε αυτούς και μερικά ακόμα χαρακτηριστικά που δεν κόβουν πολλές στήλες το καθένα από μόνο του αλλά έχουν σχεδόν 100% σταστιστική επαλήθευση τότε έχουμε:
561832/1221759 δηλ. 46,0% με επαλήθευση 1337/2291 δηλ. 58,4% και 27,0% μεγαλύτερη στατιστική επαλήθευση.
Βασικά παίζοντας τις 46 στις 100 του συνόλου των στηλών θα είχαμε κερδίσει 58 φορές στις 100.
Ετσι το web app αυτό μας βρίσκει αυτές τις στήλες... και λοιπόν? τι να τις κάνουμε? Μπορείτε να τις παίζετε σε κάθε κλήρωση? Οχι βέβαια μια και κανένας δεν έχει και ούτε θέλει να ξοδεύει τόσα χρήματα σε κάθε κλήρωση αλλά και περισσότερο να συμπληρώνει όλα αυτά τα περίπου 100.000 δελτία για να κερδίσει το Τζόκερ. 
Ο σκοπός λοιπόν είναι να δημιουργηθεί μια κοινότητα από χρήστες της εφαρμογής π.χ. 10.000 χρήστες οι οποίοι να είναι διατεθιμένοι να παίζουν 10-50 στήλες από αυτές, τυχαία επιλεγμένα με τρόπο ώστε ο καθένας να παίρνει διαφορετικές και να παίζονται κάποιες από αυτές και θα δούμε κάποιους από αυτούς τους χρήστες να κερδίζουν το Τζόκερ περίπου 6 στις 10 φορές σύμφωνα με την παραπάνω στατιστική επαλήθευση και αν τις μοιράζονταν όλες μεταξύ τους. 

Για παράδειγμα αν είχε ξεκινήσει η προσπάθεια αυτή από τον Οκτώβριο του 2020 θα είχαμε πιάσει το Τζόκερ με τις παρακάτω κληρωθήσες στήλες
2276   1/10/2020    5   11   30   41   44   20    
2277   4/10/2020    2   16   24   32   36   16   
2278   6/10/2020    3    4    7   11   45    4   
2280  11/10/2020    5   14   42   43   45   10    
2281  13/10/2020   11   17   27   35   38   20   
2282  15/10/2020    2   31   33   36   37   18  
2284  20/10/2020   17   19   22   23   38   14   
2285  22/10/2020   11   17   20   34   43   10  
2287  27/10/2020    6    8   17   30   37    8  
2288  29/10/2020    9   24   26   31   35    4    
2289   1/11/2020    4    6   22   26   30    2    
2290   3/11/2020    9   12   31   32   35   10  
δηλ ήδη 12 φορές.

Υπάρχει και ένα χαρακτηριστικό ακόμα που κόβει πάρα πολλές στήλες αλλά με κόστος και την  στατιστική επαλήθευση γι αυτό όποιος θέλει να τον βάλει και ζητάει τέτοιες στήλες θα μπορεί να το κάνει μόνος του. Το ποιές και πόσες στήλες θα μείνουν εξαρτάται από το ποιοί αριθμοί κληρώθηκαν την τελυταία φορά
Για την επόμενη κλήρωση μας δίνει 459.931 δηλ.το 37,6% και 40,9% επαλήθευση.
2277   4/10/2020    2   16   24   32   36   16  
2278   6/10/2020    3    4    7   11   45    4  
2280  11/10/2020    5   14   42   43   45   10  
2282  15/10/2020    2   31   33   36   37   18   
2284  20/10/2020   17   19   22   23   38   14 
2285  22/10/2020   11   17   20   34   43   10 
2287  27/10/2020    6    8   17   30   37    8  
2288  29/10/2020    9   24   26   31   35    4   
2289   1/11/2020    4    6   22   26   30    2  
δηλ. 9 φορές από αρχές Οκτώβρη.

Ελάτε λοιπόν ζητήστε κάποιες στήλες δίνοντας απλά το email σας και το πλήθος των στηλών που θέλετε και παίξτε τες γνωρίζοντας ότι κανένας άλλος δεν θα τις έχει. Το email σας δεν αποθηκεύεται πουθενά απλά χρειάζεται για να σας αποσταλεί από την εφαρμογή ένα αρχείο που θα λέγεται stiles_jkr.csv με τις στήλες που διαλέχτηκαν για σας.
Το μόνο που θα ξέρει η εφαρμογή είναι το σύνολο των στηλών που ζητήθηκαν και θα ανακοινώνει μετά από κάθε κλήρωση τις επιτυχίες από το σύνολο των στηλών που μοιράστηκαν.
Για να πάρετε τις στήλες δεν πληρώνετε τίποτα και αν κάποιος κερδίσει δεν έχει καμία υποχρέωση σε κανέναν, αλλά αν θέλει να κάνει μια δωρεά προς το site αυτό είναι θεμιτό και επιθυμητό. 
Και βέβαια εννοείται ότι τα τυχερά παιχνίδια εγκυμονούν κινδύνους εθισμού και απώλειας περιουσίας. 
Γι' αυτό παίζουμε Τζόκερ υπεύθυνα, για το παιχνίδι και μόνο και αν σου κάτσει...

Τον αριθμό Joker που συμπληρώνει κάθε στήλη είναι δικό σας αν και το site θα προτείνει 6-8 αριθμούς κάθε φορά, οπότε διαλέγετε και παίρνετε.


XD 1187286/1221759 2252/2291 0.972 0.983 1.011
SD>2 1216258 2280 0.995 0.995
NB<5,5,4,4 1204587 2266 0.986 0.989 1.003
CC<=3 1198449 2253 0.981 0.983 1.002
Co_df10>1 1187865 2236 0.972 0.976 1.004
last<=1 1114958 2086 0.913 0.911 0.998







































