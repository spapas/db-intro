# ΒΔ

## Ορισμοί

**Βάση δεδομένων (ΒΔ - database DB)** είναι *μια συλλογή από σχετιζόμενα δεδομένα*. Παραδείγματα: Τηλεφωνικός κατάλογος, κατάλογος στοιχείων μαθητών κλπ.

**Σύστημα διαχείρισης βάσεων δεδομένων (ΣΔΒΔ - Database Management System DBMS)** είναι μια συλλογή από προγράμματα τα οποία επιτρέπουν στους χρήστες να δημιουργήσουν και συντηρήσουν μια ΒΔ.

Οι τρεις κύριες λειτουργίες που παρέχει ένα ΣΔΒΔ για τις ΒΔ είναι:

- Ο ορισμός (definition) μιας ΒΔ, δηλαδή ο καθορισμός των τύπων, δομών και περιορισμών των δεδομένων της βάσης.
- Η κατασκευή (construction) μιας ΒΔ, δηλαδή ο τρόπος μέσω του οποίου τα δεδομένα αποθηκεύονται στο δίσκο.
- Ο χειρισμός (manipulation) μιας ΒΔ, δηλαδή η υποβολή ερωτημάτω, εισαγωγή / επεξεργασία των δεδομένων κλπ.

*ΒΔ + ΣΔΒΔ = Σύστημα Βάσης Δεδομένων ΣΒΔ (Database System DBS)*

## Παράδειγμα

Βάση δεδομένων **ΣΧΟΛΗ**

- ΦΟΙΤΗΤΗΣ
- ΜΑΘΗΜΑ
- ΔΙΔΑΣΚΑΛΙΑ
- ΒΑΘΜΟΛΟΓΙΑ

## Διαφορές ΒΔ από απλά αρχεία / προγράμματα

- Αυτοπεριγραφική φύση: Εκτός από τα δεδομένα περιέχεται και η περιγραφή αυτών (*μετα-δεδομένα*) πχ δομή του αρχείου, τύποι δεδομένων, περιορισμοί επί των δεδομένων.
- Απόμονωση μεταξύ προγραμμάτων και δεδομένων: Μπορεί να γίνουν αλλαγές στη μορφή των δεδομένων χωρίς να χρειάζονται αλλαγές στα προγράμματα προσπέλασης.
- Πολλαπλές όψεις των δεδομένων: Κάθε χρήστης που χρησιμοποιεί τη ΒΔ δύναται να βλέπει μιά διαφορετική όψη των περιεχομένων της (πχ να μη βλέπει κάποια δεδομένα τα οποία δε του χρειάζονται)
- Υποστήριξη πολλαπλών χρηστών: Πολλοί χρήστες μοιράζονται τα δεδομένα μιας ΒΔ και μπορούν ταυτόχρονα να ενεργούν σε αυτά.

## Ωφέλη από τη χρήση ενός ΣΔΒΔ

- Μόνιμη αποθήκευση δεδομένων: Τα προγράμματα χρησιμοποιούν τις βάσεις δεδομένων για να αποθηκεύουν τα δεδομένα τους.
- Ευελιξία στα προγράμματα: Μπορεί εύκολα να γίνει αλλαγή στη μορφή μιας Βάσης Δεδομένων χωρίς να επηρεαστούν τα προγράμματα που την χρησιμοποιούν
- Ταχύτερη ανάπτυξη προγραμμάτων: Αντί το κάθε πρόγραμμα να χρησιμοποιεί το δικό του τρόπο για να αποθηκεύει τα αρχεία του, όλα χρησιμοποιούν τη Βάση Δεδομένων
- Έλεγχος πλεονασμών: Δε χρειάζεται κάθε χρήστης των δεδομένων να διατηρεί ξεχωριστό αρχείο - η βάση δεδομένων είναι κοινή απλώς κάθε ένας βλέπει τα δεδομένα που τον αφορούν.
- Περιορισμοί ορθότητας: Μπορούν να επιβληθούν περιορισμοί ώστε να διασφαλιστεί η ορθότητα των στοιχείων που γράφονται στη ΒΔ, πχ τύποι δεδομένων, συσχετίσεις μεταξύ εγγραφών κλπ
- Περιορισμός μη εξουσιοδοτημένης πρόσβασης: Κάθε χρήστης βλέπει τα δεδομένα που τον αφορούν και μόνον αυτά.
- Πολλαπλές διεπαφές χρήστη: Τα δεδομένα είναι κοινά αλλά μπορεί να υπάρχουν πολλές διεπαφές (interfaces) μέσω των οποίον τα βλέπουν οι χρήστες
- Παροχή μηχανισμών τήρησης εφεδρικών αντιγράφων και ανάκαμψης.

## Ταξινόμηση ΣΔΒΔ

Χρησιμοποιούνται διάφορα κριτήρια:

- Ανά μοντέλο δεδομένων
  - Σχεσιακό (Relational): Το πιο δημοφιλές μοντέλο, τα περισσότερα ΣΔΒΔ βασίζονται σε αυτό. Ουσιαστικά παριστάνει μια ΒΔ ως μια συλλογή από πίνακες.
  - Μη σχεσιακό (Non-Relation, NoSQL): Περιλαμβάνει διάφορα μοντέλα δεδομένων - παρότι μη σχεσιακές βάσεις υπήρχαν αρχικά, πριν την χρησιμοποίηση του σχεσιακού μοντέλου, έχει ξαναγίνει δημοφιλές τα τελευταία χρόνια λόγω της ευκολίας που δίνει στην οριζόντια κλιμάκωση (horizontal scaling - αντίθετα οι σχεσιακές ΒΔ κλιμακώνονται συνήθως κάθετα - vertical scaling). Ορισμένα μοντέλα δεδομένων μη σχεσιακών ΣΔΒΔ:
      - Key-value stores
      - Document-oriented


- Ανά αριθμό χρηστών:
  - Ενός χρήστη (single-user)
  - Πολλαπλών χρηστών (multi-user)


- Ανά αριθμό εγκαταστάσεων
  - Συγκεντρωτικά (centralized)
distributed)


- Ανοιχτού ή κλειστού κώδικα
- Γενικού ή ειδικού σκοπού


## Ορισμένα γνωστά ΣΔΒΔ

- Ανοιχτού κώδικα
  - Sqlite (relational / single-user / centralized )
  - Mysql (relational / multi-user / συνήθως centralized)
  - Postgresql (relational / multi-user / συνήθως centralized)
  - Postgresql (relational / multi-user / συνήθως centralized )
  - Redis (non relational -- key-value store / multi-user / συνήθως distributed )
  - Mongodb (non relational -- document-oriented / multi-user / συνήθως distributed )  


- Κλειστού κώδικα
  - Microsoft Access (relational / single-user / centralized)
  - Microsoft SQL Server (relational / multi-user / συνήθως centralized)
  - Oracle (relational / multi-user / συνήθως centralized)
  - IMB DB2 (relational / multi-user / συνήθως centralized)

# Το μοντέλο οντοτήτων συσχετίσεων

Το μοντέλο Οντοτήτων Συσχετίσεων (ΟΣ - Entity Relationship ER) χρησιμοποιείται
για την υψηλού επιπέδου αναπαράσταση δεδομένων. Κάθε αντικείμενο που θέλουμε
να αναπαραστήσουμε στη βάση ονομάζεται Οντότητα (entity πχ σπουδαστής, σχολή)
και έχει μια σειρά από γνωρίσματα/ιδιότητες (attributes πχ όνομα, ηλικία). Οι
αλληλεπιδράσεις μεταξύ των οντοτήτων είναι οι συσχετίσεις τους (relashinships
  πχ ο σπουδαστής φοιτά σε σχολή).

## Τύποι οντοτήτων

Ένας **τύπος οντοτήτων** είναι ένα σύνολο από οντότητες με τα ίδια γνωρίσματα
(προσοχή όχι με τις ίδιες τιμές στα γνωρίσματα) και αναπαρίσταται στο ΟΣ
διάγραμμα με ένα παραλληλόγραμμο. Όλες οι οντότητες ενός τύπου οντοτήτων
σε μια ΒΔ ονομάζεται **σύνολο οντοτήτων**. Κάθε τύπος οντότητας μπορεί
να έχει γνωρίσματα τα οποία διακρίνονται σε:

- Απλά ή σύνθετα (όνομα / ονοματεπώνυμο)
- Μονότιμα ή πλειονότιμα (μέγεθος / χρώματα ρούχου)
- Αποθηκευμένα ή παραγόμενα (ημ. γέννησης / ηλικία)
- Null (δεν έχει τιμή ή δε ξέρουμε την τιμή ή δεν έχει νόημα η τιμή)

Τα απλά γνωρίσματα για κάθε οντότητα παίρνουν τιμές από 
το **σύνολο τιμών (value set)** ή **πεδίο ορισμού (domain)** τους.
Για παράδειγμα, αν ένας εργαζόμενος μπορεί να είναι από 16 ως 70 ετών
το σύνολο τιμών του γνωρίσματος ηλικία του τύπου οντότητας ΕΡΓΑΖΟΜΕΝΟΣ
προσδιορίζεται ως το σύνολο των ακεραίων μεταξύ 16 και 70.

Τα γνωρίσματα αναπαρίστανται ως ελλείψεις που
συνδέονται με ευθεία γραμμή με τον τύπο οντότητας, ενώ τα πλειότιμα
γνωρίσματα παρουσιάζονται σαν ελλείψεις με διπλό περίγραμμα.

Ένας σημαντικός περιορισμός για τις οντότητες ενός τύπου οντοτύτων
είναι ο **περιορισμός μοναδικότητας ή κλειδιού (uniqueness/key constraint)**:
Ένας τύπος οντοτήτων μπορεί να έχει κάποιο γνώρισμα το οποίο
έχει διακεκριμμένες τιμές για κάθε ξεχωριστή οντότητα (πχ ΑΜ φοιτητή, ΑΜΚΑ εργαζομένου,
ΑΦΜ φυσικού προσώπου, Αρ. πλαισίου αυτοκινήτου, ΙΜΟ πλοίου κοκ) (δηλαδή δε μπορεί να
υπάρχουν δύο διαφορετικές οντότητες με ίδιες τιμές στο συγκεκριμένο γνώρισμα
ή αντίστοιχα, εφόσον δύο οντότητες έχουν την ίδια τιμή στο συγκεκριμένο γνώρισμα συνεπάγεται
ότι είναι οι ίδιες οντότητες). Το συγκεκριμένο
γνώρισμα μπορεί να χρησιμοποιηθεί για να προσδιορίσει μια οντότητα
και λέγεται γνώρισμα-κλειδί. Μπορεί να χρειάζονται παραπάνω από ένα γνώρισμα
για να προσδιοριστεί μοναδικά ένας τύπος οντοτήτων (πχ ΑΜ φοιτητή / σχολή που φοιτά)
τότε το σύνθετο γνώρισμα που περιλαμβάνει αυτά τα γνρίσματα αυτό είναι το γνώρισμα-κλειδί 
του τύπου οντοτήτων.

## Τύποι συσχέτισης

Ένας τύπος συσχέτισης (relationship type) μεταξύ n τύπων οντοτήτων ορίζει
ένα σύνολο συνδέσεων / συσχετίσεων μεταξύ αυτών και αναπαραίσταται με ένα
ρόμβο που συνδέεται τους σχετιζόμενους τύπους οντοτήτων. Συνήθως οι τύποι
συσχέτισης συνδέοουν δύο οντότητες (είναι δηλαδή βαθμού δύο - δυαδικοί) πχ
ο τύπος συσχέτισης ΕΡΓΑΖΕΤΑΙ μεταξύ των ΕΡΓΑΖΟΜΕΝΟΣ και ΤΜΗΜΑ. Ένα παράδειγμα
τύπου συσχέτισης βαθμού τρία (τριαδικός) είναι ο τύπος συσχέτισης ΠΡΟΜΗΘΕΥΕΙ
μεταξύ των ΠΡΟΜΗΘΕΥΤΗΣ, ΑΝΤΙΚΕΙΜΕΝΟ, ΕΤΑΙΡΕΙΑ. 

Ένα γνώρισμα μπορεί να θεωρηθεί ως συσχέτιση: Παράδειγμα ένα γνώρισμα με όνομα
ΚΩΔ_ΤΜΗΜΑΤΟΣ του ΕΡΓΑΖΟΜΕΝΟΣ ή ένα (πλειότιμο) γνώρισμα ΕΡΓΑΖΟΜΕΝΟΙ του ΤΜΗΜΑ 
(προσοχή: το ένα είναι αντίστροφο του άλλου) μπορούν να αναπαραστήσουν τον τύπο 
συσχέτισης ΕΡΓΑΖΕΤΑΙ.

Οι τύποι οντοτήτων που συμμετέχουν σε ένα τύπο συσχέτισης παίζουν ένα
συγκεκριμένο ρόλο (role). Για παράδειγμα, στον τύπο συσχέτισης ΕΡΓΑΖΕΤΑΙ
οι ρόλοι είναι οι εργαζόμενος (ΕΡΓΑΖΟΜΕΝΟΣ ) και εργοδότης (ΤΜΗΜΑ). Οι ρόλοι
κυρίως έχουν σημασία σε αναδρομικούς τύπους συσχετίσεων (δηλαδή όταν ο ίδιος
τύπος οντοτήτων συμμετέχει περισσότερες από μία φορά σε ένα τύπο συσχετίσεων)
αφού σε μη αναδρομικούς τύπος συσχετίσεων φαίνεται ξεκάθαρα ποιος είναι ο
ρόλος κάθε οντότητας που συμμετέχει στη συσχέτιση.
Για παράδειγμα ο τύπος συσχετίσης ΕΠΙΒΛΕΠΕΙ συσχετίζει τον τύπο οντοτήτων
ΕΡΓΑΖΟΜΕΝΟΣ με τον εαυτό του, μια φορά με το ρόλο προϊστάμενος και μια ακόμα
με το ρόλο υφιστάμενος.

Ο λόγος πληθικότητας για δυαδικές συσχετίσεις (cardinality ratio) προσδιορίζει
τον αριθμό των στιγμιοτύπων μιας συσχέτισης στα οποία μπορεί να συμμετέχει μια οντότητα.
Οι συνήθεις λόγοι πληθικότητας είναι 1:1, 1:Ν, Ν:1 και Μ:Ν. Παραδείγματα:

  - Ο τύπος συσχέτισης ΕΡΓΑΖΕΤΑΙ μεταξύ ΤΜΗΜΑ και ΕΡΓΑΖΟΜΕΝΟΣ έχει λόγο πληθικότητας 1:Ν (ήτοι ένα τμήμα έχει πολλούς εργαζόμενος αλλά ένας εργαζόμενος εργάζεται σε ένα μόνον τμήμα) 
  - Ο τύπος συσχέτισης ΕΡΓΑΖΕΤΑΙ μεταξύ του ΕΡΓΑΖΟΜΕΝΟΣ και ΤΜΗΜΑ έχει λόγο πληθικότητα Ν:1, δηλαδή το 1:Ν είναι ταυτόσημο με το Ν:1 ανάλογα με το πώς διαβάζεται η συσχέτιση
  - Ο τύπος συσχέτισης ΑΠΑΣΧΟΛΗΣΗ μεταξύ του ΕΡΓΑΖΟΜΕΝΟΣ και ΕΡΓΟ έχει λόγο πληθικότητα Μ:Ν (ήτοι ένας εργαζόμενος συμμετέχει σε πολλά έργα αλλά και ένα έργο υλοποιείται από πολλούς εργαζόμενους)
  - Ο τύπος συσχέτισης ΔΙΕΥΘΥΝΕΙ μεταξύ του ΕΡΓΑΖΟΜΕΝΟΣ και ΤΜΗΜΑ είναι 1:1 (ήτοι ένα τμήμα έχει ένα διευθυντή και ένας εργαζόμενος μπορεί να διευθύνει ένα τμήμα)

Ο περιορισμός συμμετοχής για συσχετίσεις περιγράφει το αν είναι απαραίτητο
ή όχι ένας τύπος οντοτήτων να συμμετέχει σε ένα τύπο συσχέτισης. Συγκεκριμένα,
στην περίπτωση της μερικής συμμετοχής, ένας τύπος οντοτήτων μπορεί να συμμετέχει
προαιρετικά σε μια συσχέτιση, αντίθετα, στην περίπτωση της ολικής συμμετοχής
είναι απαραίτητη η συμμετοχή του τύπου οντοτήτων στον τύπο συσχέτισης. Ως παράδειγμα,
στον τύπο συσχέτισης ΕΠΙΒΛΕΠΕΙ ο τύπος οντότητας ΕΡΓΑΖΟΜΕΝΟΣ συμμετέχει από τη
μία μερικώς (με το ρόλο του προϊσταμένου αφού δεν είναι όλοι οι εργαζόμενοι
προϊστάμενοι) και από την άλλη ολικώς (αφού όλοι οι εργαζόμενοι έχουν κάποιο
προϊστάμενο -- έστω τον εαυτό τους στην περίπτωση του διευθυντή). Άλλο παράδειγμα,
στον τύπο συσχέτισης ΕΡΓΑΖΕΤΑΙ μεταξύ του ΤΜΗΜΑ και ΕΡΓΑΖΟΜΕΝΟΣ και οι δύο τύποι οντότητας
συμμετέχουν ολικά στη συσχέτιση αφού κάθε τμήμα πρέπει να έχει εργαζόμενους και
κάθε εργαζόμενος πρέπει να ανήκει σε κάποιο τμήμα. Αντίθετα, στον τύπο συσχέτισης
ΔΙΕΥΘΥΝΕΙ μεταξύ ξανά του ΤΜΗΜΑ και ΕΡΓΑΖΟΜΕΝΟΣ ο τύπος οντότητας ΕΡΓΑΖΟΜΕΝΟΣ
συμμετέχει μερικώς ενώ ο τύπος οντότητας τμήμα συμμετέχει ολικά (γιατί;). Η ολική συμμετοχή
ενός τύπου οντοτήτων σε ένα τύπο συσχέτισης παρουσιάζεται στο ER διάγραμμα με
μια διπλή γραμμή.

Οι τύποι συσχετίσεων μπορεί και αυτοί να έχουν γνωρίσματα. Για παράδειγμα
στον τύπο συσχέτισης ΑΠΑΣΧΟΛΗΣΗ μπορεί να περιλάβουμε ένα γνώρισμα ώρες για
τις ώρες που συμμετείχε ο ΕΡΓΑΖΟΜΕΝΟΣ στο ΕΡΓΟ. Άλλο παράδειγμα είναι το γνώρισμα
ημερομηνία έναρξης για τον τύπο συσχέτισης ΔΙΕΥΘΥΝΕΙ. Τα γνωρίσματα των 1:1
τύπων συσχετίσεων μπορούν να μεταφερθούν σε έναν από τους συμμετέχοντες
τύπους. Για παράδειγμα στη συσχέτιση ΔΙΕΥΘΥΝΕΙ, το ημερομηνία έναρξής 
μπορεί να είναι γνώρισμα είτε του ΕΡΓΑΖΟΜΕΝΟΣ είτε του ΤΜΗΜΑ (καλύτερα όμως 
στο ΤΜΗΜΑ - γιατί;). Για τους 1:Ν
τύπους συσχετίσεων το γνώρισμα μπορεί να μεταφερθεί μόνον στην πλευρά του Ν,
για παράδειγμα, στη στον τύπο συσχετίσης ΕΡΓΑΖΕΤΑΙ, το γνώρισμα ημερομηνία
έναρξης μπορεί να μεταφερθεί μόνον στην πλευρά του ΕΡΓΑΖΟΜΕΝΟΣ (και όχι στο
ΤΜΗΜΑ - γιατί;). Το γνώρισμα ώρες όμως του Μ:Ν τύπου συσχετίσεων ΕΡΓΟ
δε μπορεί να μεταφερθεί σε κανένα τύπο οντοτήτων αλλά πρέπει να παραμείνει στον
τύπο συσχέτισης (γιατί;).

![ER](er.png?raw=true "ER")



