# fce-manifest

Fandom Content Engine 업데이트 매니페스트.

앱이 시작할 때 `manifest.json`을 읽어 새 버전이 있는지 확인한다
(`edition.py`의 `UPDATE_MANIFEST_URL`).

    https://raw.githubusercontent.com/1000is0/fce-manifest/main/manifest.json

**이 주소는 출고된 모든 버전에 박혀 있다.** 레포 이름·파일명·브랜치를 바꾸면
이미 설치된 앱들이 업데이트 확인을 영구히 못 하게 된다.

파일은 손으로 고치지 않는다 — `build.py --edition both --publish`가 생성해서 올린다.
담기는 값은 버전, 릴리스 노트, 다운로드 페이지 주소, zip의 sha256뿐이며 비밀은 없다.
