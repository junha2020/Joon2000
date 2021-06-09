#include <string>
#include <vector>
#include <iostream>

using namespace std;

vector<int> solution(int n, int m) {
    vector<int> answer;
    
    int max = n > m ? n : m;
    int min = n > m ? m : n;
    int maxN = 1;
    int minN = 1;
    
    for (int i = min; i >= 1; i--)
    {
        if (n % i == 0 && m % i == 0)
        {
            maxN = i;
            break;
        }
    }
    
    for (int i = max; i <= n * m; i++)
    {
        if (i % n == 0 && i % m == 0)
        {
            minN = i;
            break;
        }
    }
    
    answer.push_back(maxN);
    answer.push_back(minN);
    
    return answer;
}

int main() {
    int n, m;
    cin >> n >> m;
    vector<int> testAnswer = solution(n, m);
}
