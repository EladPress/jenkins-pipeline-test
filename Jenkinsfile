@Library('shared-lib@prd')_

podLauncher(
    [
        genStage(
            title: 'test',
            containerName: 'custom-image',
            commands: ['echo test']
        )
    ],
    [
        customContainerTemplates: [
            [
                name: "custom-image",
                image: 'redhat/ubi9',
                alwaysPullImage: "true"
            ]
        ]     
    ]
).call()