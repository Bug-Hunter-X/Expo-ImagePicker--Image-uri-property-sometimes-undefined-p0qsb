# Expo ImagePicker URI Undefined Bug

This repository demonstrates a bug in Expo's ImagePicker library where the `uri` property of the selected image is sometimes undefined. This issue causes unexpected crashes or errors in applications relying on the selected image's URI.

## Problem Description
The `launchImageLibraryAsync` function from `expo-image-picker` occasionally returns an image object with a null or undefined `uri` property.  This behavior is non-deterministic and makes debugging challenging.

## Solution
The proposed solution involves adding robust error handling and null checks to account for this unexpected behavior.  We verify the `uri` property before using it, preventing crashes and providing more graceful error handling.