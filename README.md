# PW-Skill-MOCK--TEST-Solution
PW Skill MOCK- TEST Solution 

// solution 1
int main() {
    int n;
    cin>>n;
    int arr[n];
    for(int i=0;i<n;i++){
        cin>>arr[i];
    }
    int n = sizeof(arr)/sizeof(arr[0]); 
    int j=0;
    while(j<n){
        if(arr[j]==0){
            for(int i = j;i<n-1;i++){
               swap(arr[i], arr[i+1]);
            }
        }
        j++; 
    }
    return 0; 
}


// solution 2
int main(){
    string str ;
    cin>>str; 
    unordered_map<char,int> m; 
    int n= str.size();
    for(int i=0;i<n;i++){
        m[str[i]]++;
    }
    int idx = -1; 
    for(int i=0;i<n;i++){
        if(m[str[i]]==1){
            idx= i; 
            break; 
        }
    }
    cout<<idx; 
    
    return 0;
}
