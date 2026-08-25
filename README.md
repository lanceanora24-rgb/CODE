#include <iostream>
#include <string>

int main() {
    int mainChoice, subChoice, dirChoice;
    std::string dirName;

    while (true) {
        std::cout << "MAIN MENU\n";
        std::cout << "----------------\n";
        std::cout << "1. To Display List of Files\n";
        std::cout << "2. To Create New Directory\n";
        std::cout << "3. To Change the Working Directory\n";
        std::cout << "4. Exit\n";
        std::cout << "Enter the Number: ";
        std::cin >> mainChoice;

        if (mainChoice == 1) {
            std::cout << "\nLIST FILE DETAIL\n";
            std::cout << "--------------------------\n";
            std::cout << "1. List All Files\n";
            std::cout << "2. List of Extension Files\n";
            std::cout << "3. List of Name Wise\n";
            std::cout << "Enter the Number: ";
            std::cin >> subChoice;

            if (subChoice == 1) {
                std::cout << "\nList of All (*.*) Files\n";
                
                std::cout << "file1.txt\n";
                std::cout << "file2.cpp\n";
                std::cout << "report.doc\n";
                std::cout << "image.jpg\n";
                std::cout << "(continues...)\n\n";
                std::cout << "Total Files: 4\n";
            }
            
        } else if (mainChoice == 2) {
            std::cout << "\nEnter the Directory name: ";
            std::cin >> dirName;
            std::cout << "Current directory: C:\\Users\\UserName\\Documents\n";
            std::cout << dirName << " Directory Successfully Created\n";
        } else if (mainChoice == 3) {
            std::cout << "\n1..back\n2..root\n3..path\n";
            std::cout << "Enter the Number: ";
            std::cin >> dirChoice;
           
        } else if (mainChoice == 4) {
            break;
        } else {
            std::cout << "Invalid choice. Please try again.\n";
        }
        std::cout << "\nPress any key to continue...\n";
        std::cin.ignore(); 
        std::cin.get();
        std::cout << "\n";
    }

    return 0;
}
