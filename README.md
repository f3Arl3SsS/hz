from PyQt5.QtCore import Qt 
from PyQt5.QtWidgets import QVBoxLayout, QHBoxLayout, QMessageBox, QRadioButton, QApplication, QWidget, QLabel 
 
app = QApplication([]) 
main_win = QWidget() 
victory = QMessageBox() 
victory.setText('Верно!') 
 
question = QLabel('В каком году была создана Алгоритмика?') 
btn_answer1 = QRadioButton('2010') 
btn_answer2 = QRadioButton('2013') 
btn_answer3 = QRadioButton('2016') 
btn_answer4 = QRadioButton('2019') 
 
lineV = QVBoxLayout() 
line1 = QHBoxLayout() 
line2 = QHBoxLayout() 
line3 = QHBoxLayout() 
 
line1.addWidget(question, alignment = Qt.AlignCenter) 
line2.addWidget(btn_answer1, alignment = Qt.AlignCenter) 
line2.addWidget(btn_answer2, alignment = Qt.AlignCenter) 
line3.addWidget(btn_answer3, alignment = Qt.AlignCenter) 
line3.addWidget(btn_answer4, alignment = Qt.AlignCenter) 
lineV.addLayout(line1) 
lineV.addLayout(line2) 
lineV.addLayout(line3) 
 
main_win.setLayout(lineV) 
 
main_win.show() 
app.exec_()

