# linux_setting
리눅스 설정 파일 및 zsh 설정 방법


## 설치
### zsh 설치
sudo apt install zsh -y 
### 쉘 변경 
sudo chsh -s /bin/zsh
 또는
chsh -s $(which zsh)
또는
sudo vim /etc/passwd 
에서 해당 하는 사용자: bash 혹은 csh을 zsh로 변경
oh my zsh 설치:  (다음 줄 전체가 한 명령. 줄바꿈없이 실행)
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

## 추가 플러그인 설치

zsh-autosuggestions 설치방법

## 경로로 들어가서 git clone 받기
cd ~/.oh-my-zsh/plugins 
git clone https://github.com/zsh-users/zsh-autosuggestions.git

## echo 명령어 사용
echo "source ${(q-)PWD}/plugins/zsh-autosuggestions/zsh-autosuggestions.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc

## .zshrc의 plugins 부분에 추가해주기 : 아래 5번 참조
vi ~/.zshrc
plugins=(git ... zsh-autosuggestions)

### vi ~/.zshrc 수정
https://github.com/wonhyukc/shell_linux/blob/main/.zshrc  를 참조
