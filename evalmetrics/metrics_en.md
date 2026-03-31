# 1. Attribute_Modification

## Instruction Adherence
* Score 5: Only the specified object is precisely modified; color, material, gloss, and other attributes fully match the instruction; the shape is 100% preserved; no unintended edits.
* Score 4: All specified objects are modified, and only their attributes are changed; the shape is preserved; there are minor deviations in color, material, or degree.
* Score 3: The object and attributes are generally correct, but there are large errors in tone, brightness, or texture; minor irrelevant edits exist; visible jagged edges or distortion.
* Score 2: The correct object is edited but the attribute value or direction is incorrect; only part of the content is modified; other objects are also unintentionally changed; slight stretching or cropping exists.
* Score 1: The target object is not modified, the wrong object is edited, or the geometric shape is altered.

## Visual Seamlessness
* Score 5: No detectable editing traces; colors and materials are fully integrated with the scene lighting and shading; the edited region is almost imperceptible.
* Score 4: The overall style is consistent with smooth transitions; only slight edge artifacts are visible when zoomed in.
* Score 3: The overall tone is normal, but local tone or grain conflicts exist; edges appear blurry; inconsistencies are noticeable.
* Score 2: Obvious edge smearing or color bleeding; abrupt changes in resolution or tone; clipped highlights or shadows; visible background defects or holes.
* Score 1: Severe color bleeding, mosaic artifacts, or heavy noise; the image is nearly unusable.

## Physical and Detail Fidelity
* Score 5: Excellent physical realism, including fine micro-highlights, diffuse light bounce, and subsurface scattering; overall scene realism is enhanced.
* Score 4: The edited material interacts realistically with the scene; shadows, highlights, and reflections are properly handled; original details are preserved.
* Score 3: Lighting, perspective, and object-ground contact are generally correct; minor acceptable flaws exist; the background is only locally affected.
* Score 2: Missing shadows or highlights; incorrect reflection direction; obvious background discoloration or distortion.
* Score 1: Objects appear floating or intersecting, or there are severe perspective or lighting inconsistencies; the background is heavily distorted.


# 2. Background_Change

## Instruction Adherence
* Score 5: The background fully matches the instruction in content, style, and placement; all foreground pixels remain unaffected.
* Score 4: The specified background is completely presented; the foreground remains intact with only minor artifacts or slight deviations from the instruction (e.g., tone differences).
* Score 3: The main background is replaced, but some elements are missing or redundant, or there is slight color spill around foreground boundaries.
* Score 2: The background is only partially replaced, or the style/content is incorrect; the foreground shows obvious unintended changes.
* Score 1: No background change, or the background is unrelated to the instruction, or the foreground is replaced or severely distorted.

## Visual Seamlessness
* Score 5: The integration is indistinguishable; edges, textures, resolution, and tone transitions are perfectly coherent.
* Score 4: Compositing traces are nearly imperceptible; texture and sharpness are consistent, with only minor issues visible when zoomed in.
* Score 3: Blending is acceptable but noticeable at close inspection, with slight edge blur, grain inconsistency, or tone shift.
* Score 2: Visible cutout halos, color or resolution mismatch, or heavy smearing artifacts.
* Score 1: Severe tearing, tone separation, or extreme blur/noise; the edited region is immediately noticeable.

## Physical Consistency (Lighting, Perspective, and Depth)
* Score 5: Physically flawless; foreground and new background are fully consistent in lighting, shadows, reflections, perspective, and atmospheric depth, enhancing overall realism.
* Score 4: Lighting, scale, depth, and camera viewpoint match well, with only minor differences.
* Score 3: Overall physically plausible, with small errors in shadow length, perspective, or environmental color.
* Score 2: Noticeable but not extreme inconsistencies in lighting, shadows, scale, or depth cues.
* Score 1: Severe mismatch, such as incorrect horizon, conflicting light directions, floating subjects, or geometric distortion.


# 3. Count Change 

## Instruction Adherence
* Score 5: Perfect execution; the number of objects exactly matches the instruction, or the target object size fully matches the specified reference.
* Score 4: Mostly correct; the object count differs by one, or the target size is close to the reference but not exactly the same.
* Score 3: The operation direction is correct, but the quantity or size is clearly incorrect (e.g., adding five when two are required; enlarging significantly when asked to shrink).
* Score 2: The wrong operation is performed (e.g., deleting when asked to add), or the correct operation is applied to the wrong object.
* Score 1: No change, the completely wrong object is edited, or the image is damaged.

## Visual Seamlessness and Naturalness
* Score 5: Completely seamless; added, removed, or resized objects are indistinguishable from the original scene, with no detectable editing traces.
* Score 4: Well integrated; editing traces are hard to notice, with only minor edge artifacts or texture inconsistency visible upon close inspection.
* Score 3: Acceptable but imperfect; edited object edges appear noticeably soft or blurred, or lighting/texture does not fully match the scene.
* Score 2: Obvious editing traces; added or resized objects show clear halos at the edges, or removed areas are filled with blurry smudges; resolution or color mismatch is visible.
* Score 1: Severe artifacts; large holes, obvious cutout traces, or heavy distortion in the edited region.

## Physical Consistency and Detail Integrity
* Score 5: Physically flawless; all edited objects are perfectly integrated into the scene’s lighting, geometry, and perspective, with all details preserved.
* Score 4: Good physical consistency; lighting, shadows, and perspective of all edited objects are correct, and resized objects preserve realistic proportions and details.
* Score 3: Generally plausible with minor errors; lighting and perspective are mostly correct, but resized object textures may appear slightly over-sharpened or blurred due to scaling.
* Score 2: Noticeable physical defects; added or resized objects have missing or incorrect shadows, or resized objects show stretching, deformation, or improper texture scaling.
* Score 1: Severe physical errors; added objects appear floating, resized objects are distorted beyond recognition, or the background is damaged.


# 4. Size Adjustment

## Instruction Adherence
* Score 5: Perfect execution; the size of the target object exactly matches the instruction or the specified reference.
* Score 4: Mostly correct; the target size is close to the reference but not exactly the same.
* Score 3: The adjustment direction is correct, but the size is clearly incorrect (e.g., significantly enlarged when only slight enlargement is required, or enlarged when asked to shrink).
* Score 2: The wrong operation is performed, or the correct size adjustment is applied to the wrong object.
* Score 1: No change, the wrong object is edited, or the image is damaged.

## Visual Seamlessness and Naturalness
* Score 5: Completely seamless; the resized object is indistinguishable from the original scene, with no detectable editing traces.
* Score 4: Well integrated; editing traces are difficult to notice, with only minor edge artifacts or texture inconsistency visible upon close inspection.
* Score 3: Acceptable but imperfect; object edges appear noticeably soft or blurred, or lighting/texture does not fully match the scene.
* Score 2: Obvious editing traces; clear halos around resized object edges, or blurry smudges in filled background areas; resolution or color mismatch is visible.
* Score 1: Severe artifacts; large holes, obvious cutout traces, or heavy distortion in the edited region.

## Physical Consistency and Detail Integrity
* Score 5: Physically flawless; the resized object is perfectly integrated into the scene’s lighting, geometry, and perspective, with all details preserved.
* Score 4: Good physical consistency; lighting, shadows, and perspective are correct, and the resized object preserves realistic proportions and details.
* Score 3: Generally plausible with minor errors; lighting and perspective are mostly correct, but textures may appear slightly over-sharpened or blurred due to scaling.
* Score 2: Noticeable physical defects; missing or incorrect shadows, or the resized object shows stretching, deformation, or improper texture scaling.
* Score 1: Severe physical errors; the object appears distorted beyond recognition, floating, or the background is damaged.


# 5. Extraction

## Object Selection and Identity
* Score 5: The specified object is precisely extracted, complete, and fully consistent with the original instance (identity).
* Score 4: The object is complete and its identity is clear; only minor extraction deviations exist (e.g., small tips such as antenna ends).
* Score 3: The object is generally correct but contains small missing or extra parts; the identity remains recognizable.
* Score 2: The category is correct but only part of the object is extracted, or there is obvious interference from other elements.
* Score 1: The wrong object or multiple objects are extracted.

## Mask Accuracy and Background Purity
* Score 5: Clean anti-aliased contours with no color spill or halo; the background is perfectly pure white throughout.
* Score 4: Edges are clean and smooth; the white (#FFFFFF) background is uniform; only minor artifacts are visible when zoomed in.
* Score 3: The mask is acceptable; slight edge blur or faint halos are visible only upon close inspection.
* Score 2: Visible jagged edges or color bleeding; gray or colored patches appear in the white background.
* Score 1: Large amounts of background residue, mask holes, or non-white background dominates the image.

## Object Integrity and Visual Quality
* Score 5: Excellent quality with high-resolution details, accurate colors, and no artifacts or distortion.
* Score 4: Details are clear and colors are accurate; artifacts are negligible.
* Score 3: Overall intact but with slight blur or noise; colors are mostly preserved.
* Score 2: Moderate noise, color shift, or slight distortion; details are clearly degraded.
* Score 1: Severe blur, compression, deformation, or missing parts; the result is unusable.


#  6. Implicit Reasoning

## Implicit Reference Understanding and Execution
* Score 5: Perfect execution; the model accurately infers the target object from the implicit description and performs the required edit flawlessly.
* Score 4: The correct object is inferred and edited, but the edit contains minor defects (e.g., slight remnants after removal).
* Score 3: The wrong object is edited but is reasonably related to the implicit query (e.g., removing the ball instead of the bat), indicating partial understanding; or the correct object is inferred but the operation is executed incorrectly.
* Score 2: The model infers and edits an obviously incorrect object, indicating a lack of understanding of the implicit context.
* Score 1: No editing is performed, or the edit targets a completely random object, showing no understanding.

## Edited Region Seamlessness
* Score 5: Completely seamless; the removed or edited area is perfectly reconstructed and indistinguishable from the surrounding scene.
* Score 4: The edit blends well with the background; any inconsistencies are minor and only visible upon close inspection.
* Score 3: Editing traces are noticeable due to texture inconsistency, softened edges, or slight color mismatch in the filled region.
* Score 2: Obvious editing traces; the background reconstruction appears as blurry or mismatched patches.
* Score 1: The edited region is severely damaged, with large holes or visually distracting artifacts.

## Scene Integrity and Detail Preservation
* Score 5: Perfect integrity; the target object is cleanly edited while all surrounding context and details are fully preserved.
* Score 4: The editing scope is well controlled; all surrounding objects and background retain their original details.
* Score 3: The edit is clean but causes minor acceptable changes to nearby background or adjacent objects.
* Score 2: The edit causes noticeable distortion or detail loss in nearby unedited objects.
* Score 1: The edit severely damages surrounding objects or the overall scene structure.


# 7. Position Adjustment

## Instruction Adherence
* Score 5: Perfect execution; only the specified object is moved exactly according to the instruction to the precise new position or spatial relationship.
* Score 4: The target object is moved to the correct position; the final placement or distance has only minor deviations.
* Score 3: The movement direction of the target object is correct, but the placement, distance, or order contains obvious errors (e.g., wrong side, too far away).
* Score 2: The correct object is moved but to a completely wrong location, or its shape/size is severely distorted.
* Score 1: The target object is not moved, or the wrong object is moved.

## Visual Seamlessness (Blending and Filling)
* Score 5: Completely seamless; the moved object and reconstructed background are indistinguishable from the original scene.
* Score 4: The edit blends well; only minor edge artifacts or slight filling inconsistencies are visible when zoomed in.
* Score 3: Editing traces are noticeable; moved object edges appear soft or blurred, or background filling shows texture/noise inconsistencies.
* Score 2: Obvious cut-and-paste effects; harsh edges; background filling is blurry or has mismatched texture/color.
* Score 1: The image is severely damaged; the moved object or background has extensive artifacts.

## Physical and Spatial Integrity
* Score 5: Physically flawless; lighting, shadows, reflections, and perspective at the new position are fully coherent, maintaining or enhancing realism.
* Score 4: The moved object interacts realistically with the new environment; lighting, shadows, and proportions are correct; occlusion handled properly.
* Score 3: Overall plausible; minor errors in lighting, perspective, or contact surfaces (e.g., object not fully resting on the ground).
* Score 2: Noticeable physical defects; missing or incorrectly directed shadows; object proportions mismatch new depth; occlusion handled improperly.
* Score 1: Severe physical errors; object floating, abnormal occlusion, severe proportion/perspective errors; original scene structure damaged.


# 8. Motion Change

## Action/Pose Accuracy
* Score 5: Perfect execution; the subject's body, limbs, and head fully adopt the pose described in the instruction.
* Score 4: The specified action/pose is achieved; only minor deviations in angles, degree, or position.
* Score 3: The core intent of the action exists, but key details are incorrect (e.g., wrong head orientation, moving the wrong limb, opposite direction).
* Score 2: Pose violates anatomical principles, or only partial incorrect actions are visible.
* Score 1: No visible change, or a completely wrong action/pose is performed.

## Identity Preservation
* Score 5: Perfect retention; after motion modification, the subject's face, body, and clothing are fully consistent and undistorted.
* Score 4: The subject's identity and shape are clearly retained, with only minor changes due to new viewpoint or lighting.
* Score 3: The subject remains recognizable, but shape, clothing, or non-moving body parts show noticeable distortion.
* Score 2: Core features (face, body shape, animal patterns) change significantly during pose modification.
* Score 1: The subject's identity is completely lost; face or key body features are unrecognizable.

## Visual Consistency
* Score 5: Flawless realism; the new pose is anatomically perfect, and lighting, shadows, and texture transitions in the edited area are seamless.
* Score 4: Clean editing with correct anatomy; lighting and perspective of moved parts match the scene.
* Score 3: Overall plausible new pose, but joint movement, shadows, or minor artifacts have issues.
* Score 2: Obvious anatomical errors, proportion problems, or cutout traces around moved parts; lighting inconsistencies are noticeable.
* Score 1: Severe artifacts; repeated limbs, broken joints, or heavy distortion in the edited region.


# 9. Parallel Instruction (simultaneously modifying multiple instructions)

## Instruction Adherence
* Score 5: Perfect execution; each object fully conforms to the specified operation, and all other scene elements remain unaffected.
* Score 4: Both target objects undergo precise operations; quantity, position, or parameters have only minor deviations; no other unintended edits.
* Score 3: Both target objects are processed; each specified operation is roughly correct but lacks details (e.g., wrong color, incomplete removal).
* Score 2: Only one object is edited correctly, or both objects are edited but the operations are wrong or incomplete; other objects have incidental changes.
* Score 1: Both objects and operations do not match the instruction; wrong objects are edited or shapes are distorted.

## Visual Seamlessness
* Score 5: Completely indistinguishable integration; tone, texture, resolution, and style perfectly match the original image.
* Score 4: Smooth blending; compositing traces are hard to notice; texture and sharpness are mostly consistent.
* Score 3: Acceptable effect, but slight edge blur, tone shift, or focus misalignment is visible up close.
* Score 2: Visible halos, color or resolution mismatch, or inconsistent scaling around edited objects.
* Score 1: Severe artifacts; obvious cutout traces, heavy blur or noise; editing traces are immediately noticeable.

## Physical Consistency and Fine Detail
* Score 5: Physically flawless; shadows, highlights, reflections, depth, and textures are perfectly integrated, enhancing overall realism.
* Score 4: Lighting, perspective, and material response are highly consistent; only minor flaws visible upon close inspection.
* Score 3: Overall plausible; minor errors in shadow length, reflection angle, or texture alignment.
* Score 2: Noticeable but tolerable inconsistencies in lighting, proportion, or depth cues.
* Score 1: Severe mismatches in lighting/perspective, missing or incorrect shadows; objects floating or distorted.


# 10. Sequential Instruction

## Instruction Chain Completion
* Score 5: Perfect execution; all instructions are executed in the correct order flawlessly.
* Score 4: All instructions are executed, but one step contains a minor error (e.g., adding a bell but with the wrong color).
* Score 3: The first instruction is executed correctly, but subsequent dependent instructions fail or are omitted (e.g., creating a goat but not adding a bell).
* Score 2: The first instruction contains major errors, rendering subsequent steps invalid, or only later instructions are attempted while ignoring prerequisites.
* Score 1: No instructions are executed, or the first instruction in the dependency chain fails.

## Overall Visual Naturalness
* Score 5: Completely seamless; all edited elements appear as part of the original photo; the final image is coherent and natural.
* Score 4: Edits blend well with each other and the scene; overall image is natural, with only minor defects visible up close.
* Score 3: Individual edits are acceptable but blending is suboptimal; the final image appears slightly unnatural or inconsistent.
* Score 2: At least one edit looks poor, with visible halos, color mismatch, or other distracting artifacts affecting the overall perception.
* Score 1: Multiple edits result in visual damage or chaos; severe artifacts are present.

## Physical Consistency and Integration
* Score 5: Physically flawless; all new or edited elements perfectly integrate with each other and the scene, with lighting, shadows, and interactions consistent and accurate.
* Score 4: Edited elements are physically consistent with each other and the scene; lighting, perspective, and proportions are correct.
* Score 3: Overall plausible, but minor errors exist in element interactions or scene integration (e.g., slight deviation in the direction of a fence shadow).
* Score 2: Significant physical inconsistencies among edited elements or with the scene (e.g., the goat has no shadow but the added bell does).
* Score 1: Multiple edits result in severe physical contradictions (e.g., floating objects, conflicting light sources, broken perspective).


# 11. Portrait Enhancement

## Achievement of Editing Goals
* Score 5: Perfect execution; the specific goal or subjective target (e.g., “look more attractive”) is achieved clearly, positively, and reasonably.
* Score 4: The specified (specific or subjective) goal is mostly achieved, with minor defects (e.g., visible abs but blurry contour; chin optimized but slightly unnatural).
* Score 3: Attempted edits but results are unconvincing, exaggerated, or only partially successful.
* Score 2: Edit has no noticeable effect or the direction is incorrect (e.g., requested to look younger but appears older).
* Score 1: No edits performed, or the edit is completely unrelated to the beautification/modification instruction.

## Identity Feature Preservation
* Score 5: Perfect retention; the person is immediately recognizable, and all non-edited features (e.g., hairstyle, eye color, unique marks) are fully preserved.
* Score 4: Identity is clearly preserved; only the target attributes are modified.
* Score 3: The person is still recognizable, but some distinctive features have changed or are lost.
* Score 2: Key facial features (eyes, nose, mouth shape) are heavily modified; the person appears as someone else.
* Score 1: The person is unrecognizable; core facial structure has been replaced.

## Visual Realism and Seamlessness
* Score 5: Completely seamless and realistic; skin texture is preserved, and the edited areas integrate perfectly with the body, lighting, and anatomy.
* Score 4: High realism and good blending; any flaws are minor and only visible up close.
* Score 3: Acceptable effect but lacks realism; skin texture overly smooth, or lighting/proportions of edited areas inconsistent.
* Score 2: Edits appear obviously fake (“retouching traces”); skin blurry, lines unnatural, or obvious digital modification marks.
* Score 1: Editing effect is strange or contains severe artifacts; shapes or textures appear unnatural.


# 12. Referential Instructions

## Referential Understanding Accuracy
* Score 5: Perfect execution; the model accurately locates the object specified by a complex description and performs the required edit flawlessly.
* Score 4: The correct target is located and the operation is performed correctly, but minor deviations exist (e.g., belt color slightly pale; zebra has slight artifacts).
* Score 3: The correct target is located but the operation is executed incorrectly (e.g., replace requested but deletion performed), or the wrong object is located but the specified operation is executed on it.
* Score 2: The wrong object is edited, but it may share a simple attribute with the real target (e.g., wrong official).
* Score 1: No edits performed, or editing is applied to completely random/unrelated objects.

## Editing Execution Quality
* Score 5: Flawless effect; the object is perfectly integrated, following all lighting, shadow, reflection, and occlusion rules, enhancing realism.
* Score 4: High consistency; new/edited objects interact realistically with scene lighting, shadows, and geometry.
* Score 3: Overall plausible but minor errors exist; lighting, perspective, and shadows are mostly correct with small tolerable inconsistencies.
* Score 2: Noticeable defects; missing or clearly incorrect shadows, lighting of the object does not match the scene.
* Score 1: Severe errors; new/edited objects float, perspective/proportions are completely wrong, or surrounding scene is damaged.

## Visual Naturalness
* Score 5: Completely seamless; edited or added objects are indistinguishable from the original scene; no editing traces detectable.
* Score 4: Well blended; editing traces are hard to notice, only minor edge artifacts visible when zoomed in.
* Score 3: Acceptable effect but with noticeable defects; edge softness, slight color mismatch, or texture inconsistency reveals editing traces.
* Score 2: Editing traces obvious and rough; visible halos, resolution/color mismatch, or blurry patches.
* Score 1: Severe artifacts; edited region is damaged, distorted, or contains large noticeable holes.


# 13. Image Repair

## Repair Effectiveness
* Score 5: Perfect effect; the image is clear and sharp, noise is removed, or watermarks are completely erased without trace.
* Score 4: Mostly effective; the specified defects are nearly completely removed, with only faint residual traces.
* Score 3: Partially effective; defects are noticeably reduced but still visible and distract from perception.
* Score 2: Very limited effect; defects still dominate, only slightly mitigated.
* Score 1: Repair ineffective; specified defects (blur, noise, watermark) unchanged, or incorrect repair applied.

## Visual Naturalness and Artifact Control
* Score 5: Completely natural; no new artifacts, smudges, or unnatural patterns; image presents original high-quality appearance.
* Score 4: Overall natural; only minor artifacts visible upon close inspection or zoom.
* Score 3: Moderate visible artifacts; repaired area may have slight smudges, color banding, or inconsistent perception.
* Score 2: Noticeable disruptive artifacts; e.g., overly smooth unnatural texture (plastic-like), strong edge halos (ringing effect), or obvious patching/smudging.
* Score 1: Severe artifacts introduced; image is damaged due to new patterns, color blocks, or distortion.

## Detail and Texture Fidelity
* Score 5: Extremely high fidelity; all original details and textures are preserved, and latent details successfully restored without fabrication.
* Score 4: Details well preserved; most original details and textures remain, only the finest micro-textures may be slightly softened.
* Score 3: Moderate detail loss; some important textures softened, but main subjects and core features remain clear.
* Score 2: Significant detail loss; key features and textures heavily smoothed, simplified, or appear fake.
* Score 1: Original details completely lost; fine textures (skin, fabric, hair) entirely erased, resulting in flat or waxy appearance.


# 14. Style Transfer

## Style Fidelity
* Score 5: Complete and faithful style transfer; colors, textures, brush strokes, and lighting perfectly match the reference throughout the entire image.
* Score 4: Style covers nearly the entire image; only minor local mismatches.
* Score 3: Key style features (tone, brushwork, texture) present but unevenly distributed or inconsistent.
* Score 2: Only part of the image exhibits the style, or unrelated styles are mixed in.
* Score 1: Target style missing or clearly incorrect.

## Content Preservation
* Score 5: All objects and spatial relationships preserved; only harmless stylized deformations present.
* Score 4: Geometric shapes nearly fully preserved; only minor, non-intrusive distortions.
* Score 3: Overall structure correct; local distortions or slight omissions exist.
* Score 2: Main subject recognizable, but size, perspective, or key parts clearly wrong or missing.
* Score 1: Main objects or layout lost/distorted; original scene almost unrecognizable.

## Rendering Quality
* Score 5: High-resolution, artifact-free; brush strokes, textures, and color transitions fully natural.
* Score 4: Clear and coherent brushwork; only minor artifacts visible when zoomed in.
* Score 3: Medium quality; local blur, noise, or texture breaks, but overall acceptable.
* Score 2: Visible seams, jagged edges, color shifts; low resolution or messy brushwork.
* Score 1: Severe noise, banding, pixel corruption, or blur; image unusable.


# 15. Object Addition 

## Instruction Adherence
* Score 5: All specified attributes are correct and scene logic is coherent; only minor microscopic imperfections.
* Score 4: Main attributes correct; only slight deviations in details or 1-2 small features missing.
* Score 3: Correct category but key attributes (position, color, size, quantity, etc.) are incorrect.
* Score 2: Added object category is wrong or unrelated to the instruction.
* Score 1: No content added, or added content is damaged/invalid.

## Visual Naturalness
* Score 5: Perfectly blended; added object is indistinguishable from the original image.
* Score 4: Style nearly uniform; only minor edge issues visible when zoomed in.
* Score 3: Overall style similar, but noticeable conflicts in lighting or color; lack of harmony is perceptible.
* Score 2: Visible paste effects; severe mismatch in style, resolution, or tone.
* Score 1: Image severely damaged or filled with artifacts.

## Physical and Detail Consistency
* Score 5: Added object enhances overall realism; highlights, shadows, and environmental effects are accurate; background largely unaffected.
* Score 4: Shadows, reflections, and material interactions are realistic; no original detail lost; background minimally affected.
* Score 3: Lighting, perspective, and contact effects mostly correct; minor acceptable flaws; limited background changes.
* Score 2: Contact or occlusion poorly handled; background has slight offsets, jagged edges, or noise; noticeable background modifications.
* Score 1: Severe physical errors (floating, perspective/lighting errors); key original elements blocked; background heavily distorted.


# 16. Object Removal

## Instruction Adherence
* Score 5: Perfect removal; only the specified object is removed with no omissions; all other elements remain unaffected.
* Score 4: Only the specified object is removed; minor accidental removal of tiny/background elements or quantity errors may exist.
* Score 3: Target object mostly removed, but extra objects were deleted or remnants of the target object remain.
* Score 2: Only partially removed the target object, or deleted a different instance/category, or other objects appear in the gap.
* Score 1: No content removed, or irrelevant objects edited.

## Visual Naturalness
* Score 5: Seamless removal; traces of removal are almost undetectable.
* Score 4: Style consistent; only minor edge issues visible when zoomed in.
* Score 3: Overall acceptable, but lighting, color, or style conflicts remain; blur or noise may be visible.
* Score 2: Obvious erasure marks; color/resolution mismatched; background not restored.
* Score 1: Image severely damaged (large gaps, severe artifacts).

## Physical and Detail Integrity
* Score 5: Physically flawless and enhances realism; lighting and texture fill accurate; microscopic details preserved.
* Score 4: Background reconstruction clean; original details preserved; only minimal changes outside removed area.
* Score 3: Lighting, perspective, and contact effects mostly correct; minor acceptable flaws; background adjusted only locally.
* Score 2: Large unfilled gaps or obvious background offsets.
* Score 1: Severe physical errors (floating elements, perspective/lighting errors); key scene elements damaged; background heavily distorted.


# 17. Object Replacement

## Instruction Adherence
* Score 5: Perfect replacement; only the specified object is removed with no omissions; the new object’s category, quantity, position, scale, pose, and details fully match the instruction.
* Score 4: Correct object fully replaced; only minor attribute deviations (color, size, etc.) exist.
* Score 3: Target object mostly replaced, but other objects were modified, remnants remain, or quantity/position errors are obvious.
* Score 2: Only part of the target object replaced, or wrong category/description used.
* Score 1: Target object not replaced, or irrelevant objects edited.

## Visual Naturalness
* Score 5: Fully seamless integration; new object perfectly fits the scene; edited area unrecognizable.
* Score 4: Style nearly uniform; only minor edge artifacts visible up close; ordinary viewers cannot detect edits.
* Score 3: Basic style similar, but lighting or tone conflicts; edges blurred or noise visible.
* Score 2: Obvious paste or smear marks; severe resolution/color mismatch; background not restored.
* Score 1: Image severely damaged; new object deformed or extremely blurred.

## Physical and Detail Integrity
* Score 5: Physically flawless and enhances realism; highlights, shadows, reflections, and environmental effects precise; background unaffected.
* Score 4: New object interacts realistically with scene (including shadows, reflections, textures) and retains original details; minimal background change.
* Score 3: Lighting, perspective, and contact surfaces mostly correct; minor but acceptable errors; background only locally adjusted.
* Score 2: Missing shadows/occlusion effects; background shows major offsets or gaps.
* Score 1: Floating, penetration, severe perspective/lighting errors; key original elements damaged; background heavily distorted.


# 18. Text Modification

## Text Accuracy
* Score 5: Perfect execution; text addition, deletion, or replacement exactly matches the instruction.
* Score 4: Content basically correct but with minor spelling, capitalization, or formatting errors.
* Score 3: Correct text edited but new content has major deviations or omissions relative to the instruction.
* Score 2: Incomplete editing (e.g., only part of text deleted/modified) or content is meaningless.
* Score 1: No edit, or target text wrong, or added/modified content completely incorrect.

## Style Matching and Visual Integration
* Score 5: Perfect style match; new text’s font, size, color, perspective, and aging/lighting effects indistinguishable from real text in the image.
* Score 4: Text style (font, size, color, wear) highly consistent with surrounding context; only minor deviations.
* Score 3: Font reasonable but noticeably inconsistent with other text in image; integration acceptable but not seamless.
* Score 2: Font, color, or style obviously wrong; conflicts with image context (e.g., medieval scroll in Arial).
* Score 1: Text unreadable, severe artifacts, or style completely out of place.

## Background Integrity and Quality
* Score 5: Background perfectly restored; area behind original text fully repaired, matching surrounding texture, lighting, and patterns.
* Score 4: Background reconstructed cleanly; only extremely minor inconsistencies or softness visible up close.
* Score 3: Background repaired but obvious defects remain, e.g., pattern/texture mismatch.
* Score 2: Background reconstruction noticeable and visually distracting; blurred patches, smeared textures, or residual text traces.
* Score 1: Deletion or modification completely damages background, leaving large gaps or meaningless patterns.


# 19. Tone Transformation

## Instruction Adherence (Tone/Mood)
* Score 5: Perfect match; image fully transformed to the specified time, weather, season, or style, completely reflecting the required atmosphere.
* Score 4: Specified tone clearly achieved but with minor deviations (e.g., “snowy” but not “blizzard”; “night” effect good but lighting not dramatic enough).
* Score 3: General direction correct but execution rough or simplistic (e.g., “night” only darkened; “winter” only desaturated).
* Score 2: Target tone barely perceptible; changes too weak to convincingly reflect the instruction.
* Score 1: No tonal change, or completely wrong tone applied (e.g., requested “night” but shows “sunny day”).

## Visual Coherence and Artistic Effect
* Score 5: Transformation visually harmonious and artistic; tonal adjustments smooth, lighting expressive, all elements perfectly integrated under new tone.
* Score 4: New tone applied consistently across the image, creating a believable atmosphere; only minor visual flaws visible up close.
* Score 3: Effect applied consistently but appears simplistic or amateur; lighting flat, colors lack depth.
* Score 2: Uneven tonal application; abrupt color blocks or unnatural transitions in color/lighting.
* Score 1: Image visually damaged due to severe artifacts, banding, color separation, or heavy noise.

## Physical Realism and Detail Preservation
* Score 5: High physical fidelity; original textures preserved, new lighting generates accurate highlights and shadows on all objects, added elements perfectly integrated.
* Score 4: Realism good; original details preserved under new lighting, added atmospheric elements interact reasonably with scene.
* Score 3: Most details preserved but physical interactions missing (e.g., snow evenly covering surfaces without realistic accumulation; missing new shadows).
* Score 2: Severe detail loss, especially in dark or bright areas; new lighting inconsistent with scene geometry.
* Score 1: Original details and textures completely lost; objects flattened/blurry; added elements (e.g., snow) violate physical rules.


# 20. Viewpoint Transformation

## Viewpoint Accuracy
* Score 5: Perfect execution; camera viewpoint precisely translated, zoomed, or rotated as described. All secondary instructions also perfectly executed.
* Score 4: Viewpoint direction and type correct but magnitude slightly off; secondary edits basically correct with minor flaws.
* Score 3: Correct transformation direction/type but with obvious magnitude errors (e.g., requested zoom-in but zoomed out, translation distance too large), or viewpoint correct but secondary instructions not executed.
* Score 2: Wrong viewpoint transformation type (e.g., requested translation but scaled), or secondary instructions completely ignored (e.g., “remove truck”).
* Score 1: No viewpoint change, or change completely opposite to instruction.

## Content Consistency and Coherence
* Score 5: Perfect coherence; all original objects retain correct shape and relationships. Newly revealed content is logical and seamlessly extends the scene.
* Score 4: Scene content well preserved; only minor harmless distortions. Newly generated content is reasonable.
* Score 3: Scene’s main structure retained, but edges show noticeable distortion, deformation, or unreasonable new content.
* Score 2: Major objects severely distorted, lost, or duplicated; newly revealed areas filled with invalid content or repeated patterns.
* Score 1: Scene completely unrecognizable or logically incoherent after transformation.

## Geometric Fidelity and Visual Quality
* Score 5: Rendering flawless; new viewpoint’s geometry perfect, clear, with no visual artifacts.
* Score 4: Perspective consistent and correct; image clear with only minor artifacts visible on close inspection.
* Score 3: Overall geometry acceptable but noticeable perspective distortion or clarity loss.
* Score 2: Perspective visibly distorted; clear visual seams or resolution mismatch.
* Score 1: Severe visual artifacts; image full of cut lines, extreme blur, or noise.


# 21. Visual Effect Removal

## Effect Removal Thoroughness
* Score 5: Effect completely removed; the specified visual effect is fully eliminated from the entire image or target area with no remnants.
* Score 4: Effect mostly removed; only complex areas or edges show minor faint traces.
* Score 3: Effect partially removed; intensity noticeably reduced but large areas of obvious remnants remain.
* Score 2: Effect barely improved; intensity only slightly reduced and still dominates the image.
* Score 1: No change; the specified effect (fog, rain, snow, shadow) remains fully, or the wrong area was edited.

## Color and Image Quality Naturalness
* Score 5: Fully natural; color, contrast, and noise fully consistent with the entire image, as if the effect never existed.
* Score 4: Overall natural; repaired areas blend well in color and brightness. Only under close inspection are minor artifacts or slight color deviations visible.
* Score 3: Noticeable quality issues; repaired areas show slight color shifts, whitening, or minor blocky/smudged artifacts.
* Score 2: Effect removal appears clearly unnatural; e.g., dehazing causes oversaturation, or shadow removal results in flat, discolored, or glowing patches.
* Score 1: Result damaged; the entire image shows severe color distortion, banding, noise, or artifacts.

## Detail Restoration and Lighting Consistency
* Score 5:Physically flawless; occluded details restored with high fidelity. New lighting, highlights, and texture interactions perfectly integrated.
* Score 4: Details restored well; occluded textures and features clearly recovered. Lighting consistent with the overall scene.
* Score 3: Effect reasonable but flawed; underlying textures partially restored but lack clarity. Lighting generally correct but missing precise highlights or directional cues.
* Score 2: Severe inconsistency; restored details blurry or unrealistic. Lighting in repaired areas clearly conflicts with main light sources.
* Score 1: Underlying details completely lost; effect-covered areas appear flat and textureless. Lighting logic is chaotic.

