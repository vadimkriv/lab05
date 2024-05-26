## Laboratory work V

Данная лабораторная работа посвещена изучению фреймворков для тестирования на примере **GTest**

```sh
$ open https://github.com/google/googletest
```

## Tasks

- [ ] 1. Создать публичный репозиторий с названием **lab05** на сервисе **GitHub**
- [ ] 2. Выполнить инструкцию учебного материала
- [ ] 3. Ознакомиться со ссылками учебного материала
- [ ] 4. Составить отчет и отправить ссылку личным сообщением в **Slack**



## Report

```sh
vadim@vadim-VirtualBox:~$ export GITHUB_USERNAME=polenk0
vadim@vadim-VirtualBox:~$ alias gsed=sed
vadim@vadim-VirtualBox:~$ cd ${GITHUB_USERNAME}/workspace
vadim@vadim-VirtualBox:~/polenk0/workspace$ pushd .
~/polenk0/workspace ~/polenk0/workspace
vadim@vadim-VirtualBox:~/polenk0/workspace$ source scripts/activate
vadim@vadim-VirtualBox:~/polenk0/workspace$ git clone https://github.com/${GITHUB_USERNAME}/lab04 projects/lab05
Клонирование в «projects/lab05»...
remote: Enumerating objects: 25, done.
remote: Counting objects: 100% (25/25), done.
remote: Compressing objects: 100% (15/15), done.
remote: Total 25 (delta 4), reused 25 (delta 4), pack-reused 0
Получение объектов: 100% (25/25), 4.51 КиБ | 4.51 МиБ/с, готово.
Определение изменений: 100% (4/4), готово.
vadim@vadim-VirtualBox:~/polenk0/workspace$ cd projects/lab05
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ git remote remove origin
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ git remote add origin https://github.com/${GITHUB_USERNAME}/lab05

vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ mkdir third-party
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ git submodule add https://github.com/google/googletest third-party/gtest
Клонирование в «/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest»...
remote: Enumerating objects: 27509, done.
remote: Counting objects: 100% (47/47), done.
remote: Compressing objects: 100% (30/30), done.
Получение объектов:  19% (5227/27509), 2.50 МиБ | 4.99 МиБ/Получение объектов:  20% (5502/27509), 2.50 МиБ | 4.99 МиБ/Получение объектов:  21% (5777/27509), 2.50 МиБ | 4.99 МиБ/Получение объектов:  22% (6052/27509), 2.50 МиБ | 4.99 МиБ/Получение объектов:  23% (6328/27509), 2.50 МиБ | 4.99 МиБ/Получение объектов:  24% (6603/27509), 2.50 МиБ | 4.99 МиБ/Получение объектов:  25% (6878/27509), 2.50 МиБ | 4.99 МиБ/Получение объектов:  26% (7153/27509), 2.50 МиБ | 4.99 МиБ/Получение объектов:  27% (7428/27509), 2.50 МиБ | 4.99 МиБ/Получение объектов:  28% (7703/27509), 2.50 МиБ | 4.99 МиБ/Получение объектов:  29% (7978/27509), 2.50 МиБ | 4.99 МиБ/Получение объектов:  30% (8253/27509), 2.50 МиБ | 4.99 МиБ/Получение объектов:  30% (8518/27509), 6.53 МиБ | 6.51 МиБ/Получение объектов:  31% (8528/27509), 6.53 МиБ | 6.51 МиБ/Получение объектов:  32% (8803/27509), 6.53 МиБ | 6.51 МиБ/Получение объектов:  33% (9078/27509), 6.53 МиБ | 6.51 МиБ/Получение объектов:  34% (9354/27509), 6.53 МиБ | 6.51 МиБ/Получение объектов:  35% (9629/27509), 6.53 МиБ | 6.51 МиБ/Получение объектов:  36% (9904/27509), 6.53 МиБ | 6.51 МиБ/Получение объектов:  37% (10179/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  38% (10454/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  39% (10729/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  40% (11004/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  41% (11279/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  42% (11554/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  43% (11829/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  44% (12104/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  45% (12380/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  46% (12655/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  47% (12930/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  48% (13205/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  49% (13480/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  50% (13755/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  51% (14030/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  52% (14305/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  53% (14580/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  54% (14855/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  55% (15130/27509), 6.53 МиБ | 6.51 МиБПолучение объектов:  56% (15406/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  57% (15681/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  58% (15956/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  59% (16231/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  60% (16506/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  61% (16781/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  62% (17056/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  63% (17331/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  64% (17606/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  65% (17881/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  66% (18156/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  67% (18432/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  68% (18707/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  69% (18982/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  70% (19257/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  71% (19532/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  72% (19807/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  73% (20082/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  74% (20357/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  75% (20632/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  76% (20907/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  77% (21182/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  78% (21458/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  79% (21733/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  80% (22008/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  81% (22283/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  82% (22558/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  83% (22833/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  84% (23108/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  85% (23383/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  86% (23658/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  87% (23933/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  88% (24208/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  89% (24484/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  90% (24759/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  91% (25034/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  92% (25309/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  93% (25584/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  94% (25859/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  95% (26134/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  96% (26409/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  97% (26684/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  98% (26959/27509), 10.84 МиБ | 7.21 МиПолучение объектов:  99% (27234/27509), 10.84 МиБ | 7.21 Миremote: Total 27509 (delta 20), reused 30 (delta 11), pack-reused 27462
Получение объектов: 100% (27509/27509), 10.84 МиБ | 7.21 МиПолучение объектов: 100% (27509/27509), 12.72 МиБ | 7.46 МиБ/с, готово.
Определение изменений: 100% (20435/20435), готово.
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ cd third-party/gtest && git checkout release-1.8.1 && cd ../..
Примечание: переключение на «release-1.8.1».

Вы сейчас в состоянии «отсоединённого указателя HEAD». Можете осмотреться,
внести экспериментальные изменения и зафиксировать их, также можете
отменить любые коммиты, созданные в этом состоянии, не затрагивая другие
ветки, переключившись обратно на любую ветку.

Если хотите создать новую ветку для сохранения созданных коммитов, можете
сделать это (сейчас или позже), используя команду switch с параметром -c.
Например:

  git switch -c <новая-ветка>

Или отмените эту операцию с помощью:

  git switch -

Отключите этот совет, установив переменную конфигурации
advice.detachedHead в значение false

HEAD сейчас на 2fe3bd99 Merge pull request #1433 from dsacre/fix-clang-warnings
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ git add third-party/gtest
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ git commit -m"added gtest framework"
[master 6498e38] added gtest framework
 2 files changed, 4 insertions(+)
 create mode 100644 .gitmodules
 create mode 160000 third-party/gtest
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ gsed -i '/option(BUILD_EXAMPLES "Build examples" OFF)/a\
> option(BUILD_TESTS "Build tests" OFF)
> ' CMakeLists.txt
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ cat >> CMakeLists.txt <<EOF
> if(BUILD_TESTS)
  enable_testing()
  add_subdirectory(third-party/gtest)
  file(GLOB \${PROJECT_NAME}_TEST_SOURCES tests/*.cpp)
  add_executable(check \${\${PROJECT_NAME}_TEST_SOURCES})
  target_link_libraries(check \${PROJECT_NAME} gtest_main)
  add_test(NAME check COMMAND check)
endif()
> EOF
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ mkdir tests
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ cat > tests/test1.cpp <<EOF
> #include <print.hpp>

#include <gtest/gtest.h>

TEST(Print, InFileStream)
{
  std::string filepath = "file.txt";
  std::string text = "hello";
  std::ofstream out{filepath};

  print(text, out);
  out.close();

  std::string result;
  std::ifstream in{filepath};
  in >> result;

  EXPECT_EQ(result, text);
}
> EOF
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ cmake -H. -B_build -DBUILD_TESTS=ON
CMake Deprecation Warning at CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.5 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


-- The C compiler identification is GNU 13.2.0
-- The CXX compiler identification is GNU 13.2.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
CMake Deprecation Warning at third-party/gtest/CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.5 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


CMake Deprecation Warning at third-party/gtest/googlemock/CMakeLists.txt:42 (cmake_minimum_required):
  Compatibility with CMake < 3.5 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


CMake Deprecation Warning at third-party/gtest/googletest/CMakeLists.txt:49 (cmake_minimum_required):
  Compatibility with CMake < 3.5 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


CMake Warning (dev) at third-party/gtest/googletest/cmake/internal_utils.cmake:239 (find_package):
  Policy CMP0148 is not set: The FindPythonInterp and FindPythonLibs modules
  are removed.  Run "cmake --help-policy CMP0148" for policy details.  Use
  the cmake_policy command to set the policy and suppress this warning.

Call Stack (most recent call first):
  third-party/gtest/googletest/CMakeLists.txt:84 (include)
This warning is for project developers.  Use -Wno-dev to suppress it.

-- Found PythonInterp: /usr/bin/python3.12 (found version "3.12.3")
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD - Success
-- Found Threads: TRUE
-- Configuring done (0.6s)
-- Generating done (0.0s)
-- Build files have been written to: /home/vadim/polenk0/workspace/projects/lab05/_build
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ cmake --build _build
[  8%] Building CXX object CMakeFiles/print.dir/sources/print.cpp.o
[ 16%] Linking CXX static library libprint.a
[ 16%] Built target print
[ 25%] Building CXX object third-party/gtest/googlemock/gtest/CMakeFiles/gtest.dir/src/gtest-all.cc.o
In file included from /home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-all.cc:42:
/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-death-test.cc: In function ‘bool testing::internal::StackGrowsDown()’:
/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-death-test.cc:1224:24: error: ‘dummy’ may be used uninitialized [-Werror=maybe-uninitialized]
 1224 |   StackLowerThanAddress(&dummy, &result);
      |   ~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~
/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-death-test.cc:1214:13: note: by argument 1 of type ‘const void*’ to ‘void testing::internal::StackLowerThanAddress(const void*, bool*)’ declared here
 1214 | static void StackLowerThanAddress(const void* ptr, bool* result) {
      |             ^~~~~~~~~~~~~~~~~~~~~
/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-death-test.cc:1222:7: note: ‘dummy’ declared here
 1222 |   int dummy;
      |       ^~~~~
cc1plus: all warnings being treated as errors
gmake[2]: *** [third-party/gtest/googlemock/gtest/CMakeFiles/gtest.dir/build.make:76: third-party/gtest/googlemock/gtest/CMakeFiles/gtest.dir/src/gtest-all.cc.o] Ошибка 1
gmake[1]: *** [CMakeFiles/Makefile2:245: third-party/gtest/googlemock/gtest/CMakeFiles/gtest.dir/all] Ошибка 2
gmake: *** [Makefile:146: all] Ошибка 2
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ rm -rf _build
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ cmake --build _build
Error: /home/vadim/polenk0/workspace/projects/lab05/_build is not a directory
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ cmake -H. -B_build -DBUILD_TESTS=ON
CMake Deprecation Warning at CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.5 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


-- The C compiler identification is GNU 13.2.0
-- The CXX compiler identification is GNU 13.2.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
CMake Deprecation Warning at third-party/gtest/CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.5 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


CMake Deprecation Warning at third-party/gtest/googlemock/CMakeLists.txt:42 (cmake_minimum_required):
  Compatibility with CMake < 3.5 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


CMake Deprecation Warning at third-party/gtest/googletest/CMakeLists.txt:49 (cmake_minimum_required):
  Compatibility with CMake < 3.5 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


CMake Warning (dev) at third-party/gtest/googletest/cmake/internal_utils.cmake:239 (find_package):
  Policy CMP0148 is not set: The FindPythonInterp and FindPythonLibs modules
  are removed.  Run "cmake --help-policy CMP0148" for policy details.  Use
  the cmake_policy command to set the policy and suppress this warning.

Call Stack (most recent call first):
  third-party/gtest/googletest/CMakeLists.txt:84 (include)
This warning is for project developers.  Use -Wno-dev to suppress it.

-- Found PythonInterp: /usr/bin/python3.12 (found version "3.12.3")
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD - Success
-- Found Threads: TRUE
-- Configuring done (0.5s)
-- Generating done (0.0s)
-- Build files have been written to: /home/vadim/polenk0/workspace/projects/lab05/_build
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ cmake --build _build
[  8%] Building CXX object CMakeFiles/print.dir/sources/print.cpp.o
[ 16%] Linking CXX static library libprint.a
[ 16%] Built target print
[ 25%] Building CXX object third-party/gtest/googlemock/gtest/CMakeFiles/gtest.dir/src/gtest-all.cc.o
In file included from /home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-all.cc:42:
/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-death-test.cc: In function ‘bool testing::internal::StackGrowsDown()’:
/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-death-test.cc:1224:24: error: ‘dummy’ may be used uninitialized [-Werror=maybe-uninitialized]
 1224 |   StackLowerThanAddress(&dummy, &result);
      |   ~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~
/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-death-test.cc:1214:13: note: by argument 1 of type ‘const void*’ to ‘void testing::internal::StackLowerThanAddress(const void*, bool*)’ declared here
 1214 | static void StackLowerThanAddress(const void* ptr, bool* result) {
      |             ^~~~~~~~~~~~~~~~~~~~~
/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-death-test.cc:1222:7: note: ‘dummy’ declared here
 1222 |   int dummy;
      |       ^~~~~
cc1plus: all warnings being treated as errors
gmake[2]: *** [third-party/gtest/googlemock/gtest/CMakeFiles/gtest.dir/build.make:76: third-party/gtest/googlemock/gtest/CMakeFiles/gtest.dir/src/gtest-all.cc.o] Ошибка 1
gmake[1]: *** [CMakeFiles/Makefile2:245: third-party/gtest/googlemock/gtest/CMakeFiles/gtest.dir/all] Ошибка 2
gmake: *** [Makefile:146: all] Ошибка 2
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ rm -rf _build
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ cmake -H. -B_build -DBUILD_TESTS=ON
CMake Deprecation Warning at CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.5 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


-- The C compiler identification is GNU 13.2.0
-- The CXX compiler identification is GNU 13.2.0
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
CMake Deprecation Warning at third-party/gtest/CMakeLists.txt:1 (cmake_minimum_required):
  Compatibility with CMake < 3.5 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


CMake Deprecation Warning at third-party/gtest/googlemock/CMakeLists.txt:42 (cmake_minimum_required):
  Compatibility with CMake < 3.5 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


CMake Deprecation Warning at third-party/gtest/googletest/CMakeLists.txt:49 (cmake_minimum_required):
  Compatibility with CMake < 3.5 will be removed from a future version of
  CMake.

  Update the VERSION argument <min> value or use a ...<max> suffix to tell
  CMake that the project does not need compatibility with older versions.


CMake Warning (dev) at third-party/gtest/googletest/cmake/internal_utils.cmake:239 (find_package):
  Policy CMP0148 is not set: The FindPythonInterp and FindPythonLibs modules
  are removed.  Run "cmake --help-policy CMP0148" for policy details.  Use
  the cmake_policy command to set the policy and suppress this warning.

Call Stack (most recent call first):
  third-party/gtest/googletest/CMakeLists.txt:84 (include)
This warning is for project developers.  Use -Wno-dev to suppress it.

-- Found PythonInterp: /usr/bin/python3.12 (found version "3.12.3")
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD
-- Performing Test CMAKE_HAVE_LIBC_PTHREAD - Success
-- Found Threads: TRUE
-- Configuring done (0.6s)
-- Generating done (0.0s)
-- Build files have been written to: /home/vadim/polenk0/workspace/projects/lab05/_build
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ cmake --build _build
[  8%] Building CXX object CMakeFiles/print.dir/sources/print.cpp.o
[ 16%] Linking CXX static library libprint.a
[ 16%] Built target print
[ 25%] Building CXX object third-party/gtest/googlemock/gtest/CMakeFiles/gtest.dir/src/gtest-all.cc.o
In file included from /home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-all.cc:42:
/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-death-test.cc: In function ‘bool testing::internal::StackGrowsDown()’:
/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-death-test.cc:1224:24: error: ‘dummy’ may be used uninitialized [-Werror=maybe-uninitialized]
 1224 |   StackLowerThanAddress(&dummy, &result);
      |   ~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~
/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-death-test.cc:1214:13: note: by argument 1 of type ‘const void*’ to ‘void testing::internal::StackLowerThanAddress(const void*, bool*)’ declared here
 1214 | static void StackLowerThanAddress(const void* ptr, bool* result) {
      |             ^~~~~~~~~~~~~~~~~~~~~
/home/vadim/polenk0/workspace/projects/lab05/third-party/gtest/googletest/src/gtest-death-test.cc:1222:7: note: ‘dummy’ declared here
 1222 |   int dummy;
      |       ^~~~~
cc1plus: all warnings being treated as errors
gmake[2]: *** [third-party/gtest/googlemock/gtest/CMakeFiles/gtest.dir/build.make:76: third-party/gtest/googlemock/gtest/CMakeFiles/gtest.dir/src/gtest-all.cc.o] Ошибка 1
gmake[1]: *** [CMakeFiles/Makefile2:245: third-party/gtest/googlemock/gtest/CMakeFiles/gtest.dir/all] Ошибка 2
gmake: *** [Makefile:146: all] Ошибка 2
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ int dummy = 0
Команда «int» не найдена, но есть 29 похожих.
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ cmake --build _build --target test
Running tests...
Test project /home/vadim/polenk0/workspace/projects/lab05/_build
    Start 1: check
Could not find executable /home/vadim/polenk0/workspace/projects/lab05/_build/check
Looked in the following places:
/home/vadim/polenk0/workspace/projects/lab05/_build/check
/home/vadim/polenk0/workspace/projects/lab05/_build/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Release/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Release/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Debug/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Debug/check
/home/vadim/polenk0/workspace/projects/lab05/_build/MinSizeRel/check
/home/vadim/polenk0/workspace/projects/lab05/_build/MinSizeRel/check
/home/vadim/polenk0/workspace/projects/lab05/_build/RelWithDebInfo/check
/home/vadim/polenk0/workspace/projects/lab05/_build/RelWithDebInfo/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Deployment/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Deployment/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Development/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Development/check
home/vadim/polenk0/workspace/projects/lab05/_build/check
home/vadim/polenk0/workspace/projects/lab05/_build/check
home/vadim/polenk0/workspace/projects/lab05/_build/Release/check
home/vadim/polenk0/workspace/projects/lab05/_build/Release/check
home/vadim/polenk0/workspace/projects/lab05/_build/Debug/check
home/vadim/polenk0/workspace/projects/lab05/_build/Debug/check
home/vadim/polenk0/workspace/projects/lab05/_build/MinSizeRel/check
home/vadim/polenk0/workspace/projects/lab05/_build/MinSizeRel/check
home/vadim/polenk0/workspace/projects/lab05/_build/RelWithDebInfo/check
home/vadim/polenk0/workspace/projects/lab05/_build/RelWithDebInfo/check
home/vadim/polenk0/workspace/projects/lab05/_build/Deployment/check
home/vadim/polenk0/workspace/projects/lab05/_build/Deployment/check
home/vadim/polenk0/workspace/projects/lab05/_build/Development/check
home/vadim/polenk0/workspace/projects/lab05/_build/Development/check
Unable to find executable: /home/vadim/polenk0/workspace/projects/lab05/_build/check
1/1 Test #1: check ............................***Not Run   0.00 sec

0% tests passed, 1 tests failed out of 1

Total Test time (real) =   0.04 sec

The following tests FAILED:
	  1 - check (Not Run)
Errors while running CTest
Output from these tests are in: /home/vadim/polenk0/workspace/projects/lab05/_build/Testing/Temporary/LastTest.log
Use "--rerun-failed --output-on-failure" to re-run the failed cases verbosely.
gmake: *** [Makefile:71: test] Ошибка 8
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ _build/check
bash: _build/check: Нет такого файла или каталога
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ cmake --build _build --target test -- ARGS=--verbose

Running tests...
UpdateCTestConfiguration  from :/home/vadim/polenk0/workspace/projects/lab05/_build/DartConfiguration.tcl
UpdateCTestConfiguration  from :/home/vadim/polenk0/workspace/projects/lab05/_build/DartConfiguration.tcl
Test project /home/vadim/polenk0/workspace/projects/lab05/_build
Constructing a list of tests
Done constructing a list of tests
Updating test list for fixtures
Added 0 tests to meet fixture requirements
Checking test dependency graph...
Checking test dependency graph end
test 1
    Start 1: check
Could not find executable /home/vadim/polenk0/workspace/projects/lab05/_build/check
Looked in the following places:
/home/vadim/polenk0/workspace/projects/lab05/_build/check
/home/vadim/polenk0/workspace/projects/lab05/_build/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Release/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Release/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Debug/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Debug/check
/home/vadim/polenk0/workspace/projects/lab05/_build/MinSizeRel/check
/home/vadim/polenk0/workspace/projects/lab05/_build/MinSizeRel/check
/home/vadim/polenk0/workspace/projects/lab05/_build/RelWithDebInfo/check
/home/vadim/polenk0/workspace/projects/lab05/_build/RelWithDebInfo/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Deployment/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Deployment/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Development/check
/home/vadim/polenk0/workspace/projects/lab05/_build/Development/check
home/vadim/polenk0/workspace/projects/lab05/_build/check
home/vadim/polenk0/workspace/projects/lab05/_build/check
home/vadim/polenk0/workspace/projects/lab05/_build/Release/check
home/vadim/polenk0/workspace/projects/lab05/_build/Release/check
home/vadim/polenk0/workspace/projects/lab05/_build/Debug/check
home/vadim/polenk0/workspace/projects/lab05/_build/Debug/check
home/vadim/polenk0/workspace/projects/lab05/_build/MinSizeRel/check
home/vadim/polenk0/workspace/projects/lab05/_build/MinSizeRel/check
home/vadim/polenk0/workspace/projects/lab05/_build/RelWithDebInfo/check
home/vadim/polenk0/workspace/projects/lab05/_build/RelWithDebInfo/check
home/vadim/polenk0/workspace/projects/lab05/_build/Deployment/check
home/vadim/polenk0/workspace/projects/lab05/_build/Deployment/check
home/vadim/polenk0/workspace/projects/lab05/_build/Development/check
home/vadim/polenk0/workspace/projects/lab05/_build/Development/check

1: Test command: 
1: Working Directory: /home/vadim/polenk0/workspace/projects/lab05/_build
Unable to find executable: /home/vadim/polenk0/workspace/projects/lab05/_build/check
1/1 Test #1: check ............................***Not Run   0.00 sec

0% tests passed, 1 tests failed out of 1

Total Test time (real) =   0.00 sec

The following tests FAILED:
	  1 - check (Not Run)
Errors while running CTest
Output from these tests are in: /home/vadim/polenk0/workspace/projects/lab05/_build/Testing/Temporary/LastTest.log
Use "--rerun-failed --output-on-failure" to re-run the failed cases verbosely.
gmake: *** [Makefile:71: test] Ошибка 8
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ gsed -i 's/lab04/lab05/g' README.md
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ gsed -i 's/\(DCMAKE_INSTALL_PREFIX=_install\)/\1 -DBUILD_TESTS=ON/' .travis.yml
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ gsed -i '/cmake --build _build --target install/a\
> - cmake --build _build --target test -- ARGS=--verbose
> ' .travis.yml
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ git add .travis.yml
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ git add tests
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ git add -p
diff --git a/CMakeLists.txt b/CMakeLists.txt
index 96a361e..d69c488 100644
--- a/CMakeLists.txt
+++ b/CMakeLists.txt
@@ -4,6 +4,7 @@ set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 
 option(BUILD_EXAMPLES "Build examples" OFF)
+option(BUILD_TESTS "Build tests" OFF)
 
 project(print)
 
(1/2) Индексировать этот блок [y,n,q,a,d,j,J,g,/,e,?]? git commit -m"added tests"
Недопустимый номер: «it commit -m"added tests"»
@@ -4,6 +4,7 @@ set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 
 option(BUILD_EXAMPLES "Build examples" OFF)
+option(BUILD_TESTS "Build tests" OFF)
 
 project(print)
 
(1/2) Индексировать этот блок [y,n,q,a,d,j,J,g,/,e,?]? 
@@ -4,6 +4,7 @@ set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 
 option(BUILD_EXAMPLES "Build examples" OFF)
+option(BUILD_TESTS "Build tests" OFF)
 
 project(print)
 
(1/2) Индексировать этот блок [y,n,q,a,d,j,J,g,/,e,?]? 
@@ -4,6 +4,7 @@ set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 
 option(BUILD_EXAMPLES "Build examples" OFF)
+option(BUILD_TESTS "Build tests" OFF)
 
 project(print)
 
(1/2) Индексировать этот блок [y,n,q,a,d,j,J,g,/,e,?]? 
@@ -4,6 +4,7 @@ set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 
 option(BUILD_EXAMPLES "Build examples" OFF)
+option(BUILD_TESTS "Build tests" OFF)
 
 project(print)
 
(1/2) Индексировать этот блок [y,n,q,a,d,j,J,g,/,e,?]? y
@@ -34,3 +35,14 @@ install(TARGETS print
 
 install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/ DESTINATION include)
 install(EXPORT print-config DESTINATION cmake)
+if(BUILD_TESTS)
+  enable_testing()
+  add_subdirectory(third-party/gtest)
+  file(GLOB ${PROJECT_NAME}_TEST_SOURCES tests/*.cpp)
+  add_executable(check ${${PROJECT_NAME}_TEST_SOURCES})
+  target_link_libraries(check ${PROJECT_NAME} gtest_main)
+  add_test(NAME check COMMAND check)
+endif()
+if (CMAKE_COMPILER_IS_GNUCXX)
+    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wno-maybe-uninitialized")
+endif()
(2/2) Индексировать этот блок [y,n,q,a,d,K,g,/,e,?]? y

vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ git commit -m"added tests"
[master e076ab4] added tests
 3 files changed, 33 insertions(+), 1 deletion(-)
 create mode 100644 tests/test1.cpp
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ git push origin master
remote: Repository not found.
fatal: repository 'https://github.com/polenk0/lab05/' not found
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ git push origin master
Перечисление объектов: 35, готово.
Подсчет объектов: 100% (35/35), готово.
При сжатии изменений используется до 8 потоков
Сжатие объектов: 100% (23/23), готово.
Запись объектов: 100% (35/35), 5.60 КиБ | 5.60 МиБ/с, готово.
Всего 35 (изменений 8), повторно использовано 22 (изменений 4), повторно использовано пакетов 0
remote: Resolving deltas: 100% (8/8), done.
To https://github.com/polenk0/lab05
 * [new branch]      master -> master
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ mkdir artifacts
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ sleep 20s && gnome-screenshot --file artifacts/screenshot.png
vadim@vadim-VirtualBox:~/polenk0/workspace/projects/lab05$ popd
~/polenk0/workspace
vadim@vadim-VirtualBox:~/polenk0/workspace$ export LAB_NUMBER=05
vadim@vadim-VirtualBox:~/polenk0/workspace$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER}
Клонирование в «tasks/lab05»...
remote: Enumerating objects: 137, done.
remote: Counting objects: 100% (25/25), done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 137 (delta 18), reused 16 (delta 16), pack-reused 112
Получение объектов: 100% (137/137), 918.92 КиБ | 2.31 МиБ/с, готово.
Определение изменений: 100% (60/60), готово.
vadim@vadim-VirtualBox:~/polenk0/workspace$ mkdir reports/lab${LAB_NUMBER}
vadim@vadim-VirtualBox:~/polenk0/workspace$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
vadim@vadim-VirtualBox:~/polenk0/workspace$ cd reports/lab${LAB_NUMBER}
vadim@vadim-VirtualBox:~/polenk0/workspace/reports/lab05$ edit REPORT.md

[1]+  Остановлен    edit REPORT.md
vadim@vadim-VirtualBox:~/polenk0/workspace/reports/lab05$ gist REPORT.md

```

## Homework

### Задание
1. Создайте `CMakeList.txt` для библиотеки *banking*.
2. Создайте модульные тесты на классы `Transaction` и `Account`.
    * Используйте mock-объекты.
    * Покрытие кода должно составлять 100%.
3. Настройте сборочную процедуру на **TravisCI**.
4. Настройте [Coveralls.io](https://coveralls.io/).

## Links

- [C++ CI: Travis, CMake, GTest, Coveralls & Appveyor](http://david-grs.github.io/cpp-clang-travis-cmake-gtest-coveralls-appveyor/)
- [Boost.Tests](http://www.boost.org/doc/libs/1_63_0/libs/test/doc/html/)
- [Catch](https://github.com/catchorg/Catch2)

```
Copyright (c) 2015-2021 The ISC Authors
```
