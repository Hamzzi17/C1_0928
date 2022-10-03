# C1_0928
C프로그래밍1 0928 수업 공부

#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>
// 반복문 - while문
//int main(void)
//{ // 구구단 출력
//	int dan = 0, num = 1;
//	printf("몇 단? ");
//	scanf("%d", &dan);
//
//	while (num < 10) // 여기에 ; 붙이면 num에서 뺑글뺑글 돌아서 실행이 안 됨.
//	{
//		printf("%d x %d = %d \n", dan, num, dan * num);
//		num++;
//	}
//	return 0;
//}
//int main(void)
//{ // 구구단 전체 출력
//	int dan = 2, num = 0;
//	
//	while (dan < 10)	// 2단부터 9단까지 반복
//	{
//		num = 1;	// 새로운 단의 시작을 위해서
//
//		while (num < 10)	// 각 단의 1부터 9의 곱을 표현
//		{
//			printf("%d x %d = %2d \n", dan, num, dan * num); // 결과 두자리 정렬
//			num++;
//		}
//		dan++;	// 다음 단으로 넘어가기 위한 증가
//	}
//
//	return 0;
//}
// 문제1.프로그램 사용자로부터 양의 정수를 하나 입력 받아서, 그 수만큼 "Hello World!"를 출력하는 프로그램
//int main(void)
//{
//	int num, i = 0;
//	printf("양의 정수를 입력하시오: ");
//	scanf("%d", &num);
//
//	while(i < num)
//	{
//		printf("Hello World! ");
//		i++;
//	}
//	return 0;
//}
// 문제 2. 프로그램 사용자로부터 양의 정수를 하나 입력 받은 다음, 그 수만큼 3의 배수를 출력하는 프로그램. 예를 들어서 5를 입력 받았다면, 3 6 9 12 15를 출력.
//int main(void)
//{
//	int num = 0, i = 1;
//	printf("양의 정수를 입력하시오: ");
//	scanf("%d", &num);
//
//	while (i <= num)
//	{
//		printf("%d ", i * 3);
//		i++;
//	}
//	return 0;
//}
//int main(void)
//{
//	int num = 0, i = 1;
//	printf("배수의 개수: ");
//	scanf("%d", &num);
//
//	while (i++ < num)
//	{
//		printf("%d ", i * 3);
//	}
//	return 0;
//}
// 문제 3. 프로그램 사용자로부터 계속해서 정수를 입력 받는다. 그리고 그 값을 계속해서 더해 나간다. 이러한 작업은 프로그램 사용자가 0을 입력할 때까지 계속되어야 하며, 0이 입력되면 입력된 모든 정수의 합을 출력하고 프로그램을 종료시킨다.
//int main(void)
//{
//	int total = 0, num = 1;
//
//	while (num != 0)
//	{
//		printf("정수 입력(0 to quit): ");
//		scanf("%d", &num);
//		total += num;
//		
//	}
//	printf("입력된 정수의 총합: %d \n", total);
//	return 0;
//}
// 문제 4. 프로그램 사용자로부터 입력 받은 숫자에 해당하는 구구단을 출력하되, 역순으로 출력하는 프로그램
//int main(void)
//{ // 구구단 역순 출력
//	int dan = 0, num = 9;
//	printf("몇 단? ");
//	scanf("%d", &dan);
//
//	while (num > 0)
//	{
//		printf("%d x %d = %d \n", dan, num, dan * num);
//		num--;
//	}
//	return 0;
//}
// 문제 5. 프로그램 사용자로부터 입력 받은 정수의 평균을 출력하는 프로그램을 작성하되 다음 두 가지조건을 만족시켜야 한다.
// "먼저 몇 개의 정수를 입력할 것인지 프로그램 사용자에게 묻는다. 그리고 그 수만큼 정수를 입력 받는다."
// "평균 값은 소수점 이하까지 계산해서 출력한다.
//int main(void)
//{
//	int num = 0, num2 = 0, i = 0;
//	double total = 0.0;
//
//	printf("입력할 정수의 개수: ");
//	scanf("%d", &num);
//
//	while (i < num)
//	{
//		printf("정수 입력: ");
//		scanf("%d", &num2);
//		total += num2;
//		i++;
//	}
//	printf("입력된 정수의 평균: %f \n", total / num); // 자동 형 변화
//	return 0;
//}
// while문 중첩
//int main(void)
//{
//	int total = 0, num = 0, i = 0;
//
//	while (i < 5)
//	{
//		while (num <= 0)
//		{
//			printf("정수 입력: ");
//			scanf("%d", &num);
//		}
//		total += num;
//		num = 0;
//		i++;
//	}
//	printf("입력된 정수의 총합: %d \n", total);
//	return 0;
//}
// 0*
//int main(void)
//{
//	int i = 0, j = 0; // 행 열
//	while(i < 5)
//	{
//		while (j < i)
//		{
//			printf("0 ");
//			j++;
//		}
//		j = 0;
//		printf("*\n");
//		i++;
//	}
//	return 0;
//}
//int main(void)
//{
//	int total = 0, num = 0;
//	do
//	{
//		printf("정수 입력(0 to quit): ");
//		scanf("%d", &num);
//		total += num;
//	} while (num != 0);
//	printf("합계: %d \n", total);
//	return 0;
//}
// // 0~100 짝수의 합 2550
//int main(void)
//{
//	int total = 0, num = 2;
//	do
//	{
//		total += num;
//		num += 2;
//	} while (num <= 100);
//	printf("짝수의 합: %d", total);
//	return 0;
//}
// for문
//int main(void)
//{
//	int total = 0;
//	int i, num;
//	printf("0부터 num까지의 덧셈, num은? ");
//	scanf("%d", &num);
//
//	for (i = 0; i < num + 1; i++)
//		total += i;
//
//	printf("0부터 %d까지의 덧셈 결과: %d \n", num, total);
//	return 0;
//}
// (total=0.0; input=0.0; num=0; num++;num1++; ...) 콤마로 구분해서 한번에 초기화 가능
// for문으로 구구단
//int main(void)
//{
//	int cur, is;
//	for (cur = 2; cur < 10; cur++) // 2단부터 9단까지 반복
//	{
//		for (is = 1; is < 10; is++) // 각 단의 1부터 9까지의 곱
//			printf("%d x %d = %d \n", cur, is, cur * is);
//		printf("\n");
//	}
//	return 0;
//}
// 문제1
//int main(void)
//{
//	int total = 0;
//	int num1, num2;
//
//	printf("두 개의 정수 입력: ");
//	scanf("%d %d", &num1, &num2);
//
//	for (total = 0; num1 <= num2; num1++)
//		total += num1;
//
//	printf("num1부터 num2까지의 정수들의 총합: %d \n", total);
//	return 0;
//}
int main(void)
{ // 팩토리얼
	int total = 1;
	int n, i = 0;

	printf("정수 입력: ");
	scanf("%d", &n); // 정수 입력

	for (i = 1; i <= n; i++)
		total = total * i; // total *= i;

	printf("%d! = %d", n, total);
	return 0;
}