# 상세 프롬프트 회귀 기준

목적: 스킬이 다시 '줄거리 + generic cinematic' 수준으로 퇴행하지 않도록 최종 출력으로 점검한다. 단어 수를 늘리는 시험이 아니다. 이 문서의 연못 소재는 테스트용이며 모든 주제에 강아지·물보라·밝은 여름 룩을 복제하지 않는다.

## 핵심 입력: 연못 장면

15초, 세로 9:16, 잔잔하게 시작해서 즐겁게 끝나는 여름 영상. 연못 환경 사진, 작은 흰 강아지 사진, 은색 앞머리와 긴 땋은 머리를 가진 동일한 쌍둥이 자매의 캐릭터 시트가 있다고 사용자가 설명한다. 그러나 텍스트 테스트에는 이미지 파일이 실제 제공되지 않는다. 흰색의 불투명한 수영복, 사람 둘과 강아지 한 마리, 외형 일관성을 유지한다.

사건 순서:
- 0–4초: 연못 가장자리에서 보는 넓은 구도. 자매가 얕은 물에서 웃으며 가볍게 물장난한다.
- 4–8초: 반대편 풀밭 둑에 강아지가 나타나 물가로 달려온다. 부드럽게 따라본다.
- 8–11초: 강아지가 자매 가까운 얕은 물에 낮게 한 번 뛰어든다. 얼굴을 가리지 않는 물보라.
- 11–15초: 자매와 강아지가 함께 즐겁게 물놀이한다. 나무 반사가 보이는 안정된 넓은 구도로 끝난다.

### 금지된 지름길

'Natural daylight, soft highlights, realistic movement'라는 세 문구를 덧붙이는 것만으로 광원·재질·물리 설계를 대신하지 않는다. 캐릭터 고정과 금지사항만 풍부하고 촬영 지시가 비어 있는 출력도 실패다. 그림을 실제로 본 것처럼 형태·배경을 단정하지 않는다.

### 합격 조건

1. 이미지 미검사와 모델/모드 미확인 상태를 명시한 **조건부 상세 연출본**을 제공한다. 준비물 안내만 하고 촬영 설계를 생략하지 않는다.
2. 카메라·자매·강아지의 둑 위치와 이동 거리를 먼저 연결한다. '반대편'을 지우거나 강아지가 연못 전체를 건너뛰게 하지 않는다.
3. 네 구간과 주요 사건을 유지한다. 실행 모델에 따라 나눠 생성할 수 있으나 하나의 호출로 반드시 된다고 주장하지 않는다.
4. 실제 영문 본문에 각 컷의 프레이밍, 카메라, 초점/심도, 행동 변화, 마지막 상태가 나타난다. 공유 조건은 명확히 적용되면 반복하지 않아도 된다.
5. 밝은 여름 빛과 흰 털/은발/흰 의상의 하이라이트 가독성을 연결하고, 물의 반사·잔물결·착수 같은 재질 반응을 구체화한다.
6. 동작 준비·접촉·물결의 원인과 결과를 표현하되 짧은 컷에 불필요한 여러 행동·카메라 효과를 겹치지 않는다.
7. 원본 자료가 생기면 확인해야 할 지형과 외형을 명시한다. 실제 이미지 없이 정확한 재현이나 완성 프롬프트를 보장하지 않는다.
8. 음향은 지원이 확인되지 않으면 편집 메모로 분리한다.

## 추가 회귀 입력

- **8초 제품:** 브랜드 없는 유리병, 카메라 완전 고정, 병도 움직이지 않음. 풍부한 디테일을 위해 카메라 이동·회전·액체 붓기를 새로 만들지 않는다. 빛, 형태, 반사, 프레임 배치, 선명도와 유지 상태로 구체화한다.
- **짧은 버전 요청:** 사용자가 '영어 80단어 이내'라고 명시하면 그 제한을 지키며 핵심 구도·행동·끝 상태를 우선한다. 상세 기본값이 명시적인 간결 요청을 이기지 않는다.
- **실물 참조 없음:** 정확한 로고·병 모양을 요구하지만 사진이 없다면 합성 병을 정답처럼 제시하지 않는다. 조건부 연출안은 준비하고 정확한 외형 확정은 대기한다.

## 평가 범위

텍스트 테스트의 합격은 지침 준수와 구체성만 의미한다. 실제 영상의 얼굴 유지, 물리 시뮬레이션, 정확한 컷 시간, 미적 품질은 생성 후 따로 평가해야 한다.


## 적용 출력과 검수 반영본: 연못

별도 AI가 이 스킬을 읽고 실제 텍스트를 작성한 뒤 검수한 예시다. 초안의 '네 컷 전환' 표현을 **네 숏·세 전환**으로 바로잡았고, 반사가 풀밭 너머에 있는 듯한 표현을 수면 위치로 수정했다. 얕은 물에 선 사람이 손으로 물을 쓸 수 있도록 몸을 낮추는 동작을 명시했다. 빠진 꼬리 움직임과 참조자료별 역할도 보강했다. 수치로 과잉 정밀하게 정하지 않고 짧은 접근 거리와 낮은 도약을 중심으로 정리했다.

**상태: 레퍼런스 대기(pending reference)·미검사, 조건부 상세 연출본. 실제 모델에 바로 실행 가능한 것으로 검증하지 않았다.** 15초·9:16·여름 분위기·사건 순서는 입력 조건이다. 광원 방향과 지형 배치는 연출 가정이다. 카메라는 가까운 둑, 자매와 강아지는 반대편의 같은 물가에 배치한다. 실제 사진이 이 배치를 허용하지 않으면 구도를 조정해야 한다.

참조 준비 및 매핑:
- 연못 사진: 공간과 식생의 기준. 맞은편 둑·얕은 진입 구간이 실제로 보이는지 확인 필요.
- 강아지 사진: 외형과 털의 기준. 사진의 벽 배경은 가져오지 않음.
- 자매 캐릭터 시트: 두 인물의 같은 얼굴, 은색 앞머리, 긴 땋은 머리의 기준. 원본 화풍과 실사 연출의 호환성도 확인 필요.
- 원본 이미지는 이 텍스트 점검에 제공되지 않았다. 아래의 source 지시는 이미지를 실제 첨부한 후에만 의미가 있다. 모델의 다중 참조/다중 숏 기능은 별도 확인한다.

```text
FORMAT AND REFERENCE ROLES
A 15-second vertical 9:16 summer sequence in four shots, with three cuts around 4, 8, and 11 seconds. Use the pond source for the natural setting, the dog source only for the small fluffy white dog's appearance rather than its wall background, and the character sheets for the twins' matching facial identity, silver bangs, and long braids. Keep their coordinated, modest, opaque white swimsuits unchanged. Let small physical changes in the water carry the scene from quiet observation to shared delight.

SHARED LOOK
Bright, soft open-sky daylight from high frame-left gives the water a gentle directional sheen rather than hard glare. Preserve detail in white fur, silver hair, and white fabric without burning them into featureless highlights. Keep faces softly filled, greens natural, and skin tones neutral. Use sufficient depth of field to read the faces and waterline actions together, with the distant foliage only slightly softer. Hands and paws interrupt the reflected trees, breaking their shapes into narrow green bands that stretch outward with the ripples. After the landing, fur around the dog's paws and lower legs becomes slightly darker and clumps subtly from the water. Keep that wet state in the following shot. The mood is clear and warm, not hazy, stormy, or heavily teal-graded.

SCENE GEOGRAPHY AND CONTINUITY
The camera looks from the near bank toward the opposite shoreline. The sisters stand in the shallows immediately beside that far shoreline, center-right in frame. The dog approaches from screen-left along the grassy far bank over a short distance. It enters the shallows beside the sisters, not across the pond. Establish a gently sloping grassy edge and a shallow landing area to the sisters' screen-left, offset so the dog and its splash do not cover their faces. The landing water remains shallow enough for the small dog to stand with its head clearly above water. Maintain the same bank, screen direction, spacing, water depth, and clothing across all shots.

SHOT 1 | 0-4s | Quiet play
Begin with a wide vertical view from low on the near bank, angled slightly along the opposite shoreline. Foreground water fills the lower third, the far grass forms a middle band, and the trees rise above it; their reflections lie on the water below the far shoreline. Place both sisters center-right and leave a visible stretch of grass to their left for the dog's later approach. Keep the camera still and focus steady across the sisters and nearby shallows. The sisters smile, bend their knees and lean forward just enough to sweep their hands lightly through the shallow surface. Their feet remain planted while thin fans of water fall back and small rings travel outward. They ease their hands clear of the water near the end of the shot. Finish on the softening ripples and readable faces, without a focus search.

SHOT 2 | 4-8s | Dog approaches
Cut from the same near-bank side, retaining the left-to-right screen direction and both sisters in view. The small white dog enters on the far-left grass, tail wagging naturally, and runs the short distance toward the shallow entry point. Begin a restrained rightward pan as it enters; rotate from the same camera position without adding a dolly or zoom. Its paws press into the grass with each step, and its fluffy coat follows the body's movement with a slight lag. Keep its full body and the sisters readable with sufficient depth of field. As it reaches the edge, the dog shortens its steps and gathers its hind legs for a low jump. Ease the pan to a stop. End with the dog still on the grass, facing the landing water, and the sisters clearly to its right.

SHOT 3 | 8-11s | Low jump and contact
Cut to a slightly tighter view on the same axis, keeping the dog's entire body, the landing water, and the sisters' faces within the vertical frame. Lock the camera and maintain focus across this small group. Begin with the gathered stance from the previous shot. The dog pushes off from the low grassy edge in one short forward hop, not a high dive or a leap across the pond. Its forepaws touch first; the hind paws follow and its body briefly absorbs the landing. The contact sends a low fan of droplets outward, below and away from the sisters' faces. Small overlapping rings break the tree reflection around the landing point. The dog regains a steady standing position with its head fully above the water. Finish with its wet lower-leg fur visible and the first rings expanding, rather than starting another jump.

SHOT 4 | 11-15s | Shared delight and hold
Return to the original wide view from the near bank, not a reverse angle. Keep the dog screen-left of the sisters at the established landing spot and preserve the damp lower-leg fur. Hold the camera fixed with faces, dog, and surface interaction clearly readable. The sisters laugh and lower their hands for a small, gentle splash beside the dog; the dog shifts one front paw playfully through the water. Their low splashes fall back without hiding faces. The hand-made and paw-made ripples overlap, then widen across the green reflections. Let their movements settle around the final second. End on a steady composition of the smiling sisters, the calmly standing dog, and the reflected trees becoming readable between the fading ripples.

ESSENTIAL CONSTRAINTS
Exactly two sisters and one dog. Preserve matching faces, braids, outfits, and dog appearance. No additional people or animals, no bank switching, no deep-water dive, no jumping onto the sisters, no distorted limbs, text, or added logos. Keep motion naturally weighted without exaggerated poses.
```

음향 편집 메모: 모델의 오디오 지원을 확인하지 않았으므로 위 생성 문구와 분리한다. 잔디 위 발소리, 작은 손·발 물소리, 한 번의 낮은 착수음, 가벼운 웃음과 강아지 숨소리를 화면의 원인에 맞춘다. 대사·음악은 넣지 않는다.

실행 전: 원본 3종의 역할과 외형을 확인하고, 해당 모드의 길이·9:16·다중 이미지·다중 숏 지원과 입력 길이를 확인한다. 네 숏을 별도 생성한다면 각 호출에 필요한 참조·공통 룩·공간 정보를 함께 붙인 독립 문구로 컴파일한다. 15초와 전환 시점은 기획 목표이지 모델의 정확한 실행 보장이 아니다.

### 최종 본문에서 확인한 증거

| 기준 | 영문 상세본의 실제 구절 |
| --- | --- |
| 공간 연결 | “The dog approaches from screen-left along the grassy far bank” |
| 프레임 깊이 | “Foreground water fills the lower third” |
| 광원과 밝은 재질 | “Preserve detail in white fur, silver hair, and white fabric” |
| 초점·심도 | “maintain focus across this small group” |
| 동작의 원인·접촉 | “Its forepaws touch first; the hind paws follow” |
| 털과 물의 반응 | “clumps subtly from the water” |
| 카메라 경로와 종료 | “Ease the pan to a stop” |
| 마지막 화면 | “reflected trees becoming readable between the fading ripples” |

## 정지 제품 적용 출력

다음은 같은 스킬로 만든 정지 제품 예시다. 병의 형태와 회색 배경은 가상 제품의 연출 가정이며 특정 실물의 원본을 확인한 것이 아니다. 카메라·병을 움직이지 않고도 프레임, 반사, 그림자, 선명도를 설명한다.

```text
A single plain, clear, unbranded glass bottle with a simple neck, sloped shoulders, and a thick flat base stands upright on a matte warm-gray surface against a seamless warm-gray background. Frame the entire bottle centered with balanced negative space, in a front three-quarter view at mid-bottle height; keep it sharp from neck to base. Lock the camera and bottle completely still for all 8 seconds, ending on the identical composition: no pan, tilt, zoom, dolly, rotation, focus pull, cuts, or lighting change. A broad soft key from upper left makes one stable vertical highlight along the glass; subtle fill keeps its edges and base refraction readable, with a soft, fixed contact shadow.
```

### 사용자가 80단어 이내를 요청한 경우

아래는 별도로 편집해 68단어임을 공백 기준으로 확인한 단축 예시다. 명시적인 길이 제한이 있을 때도 핵심 촬영 정보를 우선한다.

```text
A clear unbranded glass bottle stands motionless on a warm ivory surface. Frame the whole bottle from the front at bottle height, with space around its outline. A broad soft light from upper left defines the glass edges and thick base without clipping reflections. Keep the bottle sharp, background softly separated, camera completely fixed, and lighting unchanged. Hold this composition for eight seconds; no cuts or added lettering.
```

실제 영상 생성은 세 예시 모두 수행하지 않았다. 생성 결과가 이 지시를 따르는지와 영상미가 향상되는지는 별도 렌더 비교가 필요하다.
