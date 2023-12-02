#include<stdio.h>
#define MAX_STUDENTS 50
int main(){
#define MAX_STUDENT 50
char student_name[MAX_STUDENT][50];//Array to store students names
int attendance[MAX_STUDENT]={0};//Array to store attendance(0 for absent,1 for present 
int num_student;
//Input the number of students
printf("enter the number of student\n");
scanf("%d",&num_student);
//input student name
printf("enter the name of student:\n");
for(int i =0;i<num_student;i++){
printf("student %d:",i+1);
scanf("%s",&student_name[i]);
}
//Roll call
printf("\nRoll call:\n");
for (int i=0;i<num_student;i++){
printf("is %s present?(1 for yes,0 for no):",student _name);
}
// Display attendance
printf("\nAttendance report:\n");
for (int i=0;i<num_student;i++){
printf("%s:%s\n",student _name[i], attendance[i]?"present":"absent");
}
return 0;
}
