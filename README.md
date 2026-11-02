# Hi, Hollow!

```cpp
#include <windows.h>

typedef struct _DEVELOPER_PROFILE {
    LPCWSTR Name;
    LPCWSTR Bio;
    LPCWSTR Roles[1];
    LPCWSTR Tags[3];
} DEVELOPER_PROFILE;

int WINAPI wWinMain(HINSTANCE hInstance, HINSTANCE hPrevInstance, LPWSTR lpCmdLine, int nCmdShow) {
    DEVELOPER_PROFILE me = {
        L"Hollow",
        L"-",
        { L"Cyber Security Student", },
        { L"Malware Analyst", L"Coder", L"Hacker" }
    };

    UNREFERENCED_PARAMETER(me);
    return 0;
}
