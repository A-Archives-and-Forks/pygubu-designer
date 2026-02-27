
[Leer en Español](Documentation/README/es.md). Περισσότερες Μεταφράσεις [Εδώ](Documentation/README)

Καλώς ήρθες στο Pygubu Designer!
===========================

Το `Pygubu Designer` είναι ένα εργαλείο RAD (Rapid Application Development) που επιτρέπει τη γρήγορη και εύκολη ανάπτυξη γραφικών διεπαφών χρήστη για την ενότητα `tkinter` της Python.

Οι διεπαφές χρήστη που σχεδιάζονται αποθηκεύονται ως αρχεία [XML](https://el.wikipedia.org/wiki/XML) και, χρησιμοποιώντας τον builder του pygubu, μπορούν να φορτωθούν δυναμικά από εφαρμογές όταν χρειαστεί.

Το Pygubu Designer είναι εμπνευσμένο από το [Glade](https://gitlab.gnome.org/GNOME/glade).

Εγκατάσταση
============

Η τελευταία έκδοση του pygubu απαιτεί Python >= 3.9

Μπορείτε να εγκαταστήσετε το pygubu-designer χρησιμοποιώντας το **pip**:

```
pip install pygubu-designer
```

Για άλλες μεθόδους εγκατάστασης, παρακαλώ δείτε [αυτή τη σελίδα](https://github.com/alejandroautalan/pygubu-designer/wiki/Installation-&-Related).


Στιγμιότυπο Οθόνης
==================

<img src="https://github.com/alejandroautalan/pygubu-designer/blob/master/pygubu-designer.png" alt="pygubu-desinger.png">


Χρήση
=====

Το Pygubu designer υποστηρίζει δύο τύπους ροής εργασίας. Η πρώτη και κλασική μέθοδος είναι η δημιουργία μιας εφαρμογής που χρησιμοποιεί το αρχείο "*.ui" το οποίο ορίζει τη διεπαφή χρήστη σας.

Στην κλασική λειτουργία, το pygubu είναι υπεύθυνο για τη δημιουργία των widget και τη σύνδεση των καθορισμένων δεσμεύσεων (bindings). Συνιστώ αυτή τη λειτουργία για εφαρμογές που έχουν ένα ή λίγα παράθυρα, αλλά μπορείτε να τη χρησιμοποιήσετε για τη δημιουργία εφαρμογών οποιασδήποτε πολυπλοκότητας (το ίδιο το Pygubu Designer δημιουργήθηκε με αυτή τη λειτουργία, αλλά τώρα χρησιμοποιεί τη νέα). Αυτή η μέθοδος χρησιμοποιεί μια προσέγγιση βασισμένη σε κλάσεις, όπου ο κώδικάς σας βρίσκεται στην παραγόμενη κλάση και η βασική κλάση ενημερώνεται από το pygubu designer.

Η δεύτερη μέθοδος είναι η δημιουργία μιας εφαρμογής με μια κωδικοποιημένη έκδοση του αρχείου *.ui. Χρησιμοποιώντας την ίδια προσέγγιση βασισμένη σε κλάσεις που αναφέρθηκε παραπάνω, το pygubu designer δημιουργεί τον κώδικα Python για τη βασική κλάση και εσείς γράφετε τη λογική της εφαρμογής στην παραγόμενη κλάση.

Η δημιουργία κώδικα για τη διεπαφή χρήστη έχει μερικά πλεονεκτήματα:

- Το αρχείο *.ui δεν απαιτείται κατά την εκτέλεση
- Σας επιτρέπει να δημιουργείτε καθαρές εφαρμογές tkinter, αν δεν χρησιμοποιείτε κανένα widget του pygubu (εξαλείφοντας την εξάρτηση από το pygubu).
- Εύκολη δημιουργία προσαρμοσμένων widget.

Όποια κι αν επιλέξετε, μπορείτε πάντα να τροποποιήσετε τη διεπαφή χρήστη χρησιμοποιώντας το pygubu designer.


Εκκίνηση του Pygubu Designer
------------------------

Πληκτρολογήστε στο τερματικό μία από τις παρακάτω εντολές ανάλογα με το σύστημά σας.

### Συστήματα τύπου Unix

```
pygubu-designer
```

Για άλλες πλατφόρμες δείτε [αυτή τη σελίδα](https://github.com/alejandroautalan/pygubu-designer/wiki/Launch).


Τεκμηρίωση
=============

Επισκεφθείτε το [wiki](https://github.com/alejandroautalan/pygubu-designer/wiki) για περισσότερη τεκμηρίωση.

Ακολουθούν μερικές καλές αναφορές για tkinter (και tk):

- [TkDocs](http://www.tkdocs.com)
- [Graphical User Interfaces with Tk](https://docs.python.org/3/library/tk.html)
- [Tkinter 8.5 reference: a GUI for Python](https://tkdocs.com/shipman)
- [An Introduction to Tkinter](http://effbot.org/tkinterbook) [(archive)](http://web.archive.org/web/20200504141939/http://www.effbot.org/tkinterbook)
- [Tcl/Tk 9.0 Manual](https://www.tcl-lang.org/man/tcl9.0/TkCmd/index.html)
- [Tcl/Tk 8.6 Manual](https://www.tcl-lang.org/man/tcl8.6/TkCmd/contents.htm)

Μπορείτε επίσης να δείτε τον κατάλογο [παραδειγμάτων](examples) ή να παρακολουθήσετε [αυτό το εισαγωγικό εκπαιδευτικό βίντεο](http://youtu.be/wuzV9P8geDg).


Ιστορικό
=======

Δείτε τη λίστα των αλλαγών [εδώ](HISTORY.md).


Άδεια Χρήσης
=======

Pygubu Designer: Άδεια GPL-3.0

Το Pygubu Designer μπορεί να δημιουργήσει απλά σενάρια κώδικα Python. Για εκείνες τις περιπτώσεις όπου απαιτείται άδεια για αυτά τα σενάρια, διατίθενται υπό την ίδια άδεια με τον πυρήνα pygubu: Άδεια MIT.
Αυτό ισχύει για όλα τα τυπικά πρόσθετα (plugins) που συνοδεύουν τον πυρήνα pygubu. Αν χρησιμοποιείτε πρόσθετο τρίτου κατασκευαστή, ελέγξτε την άδεια του πρόσθετου.
