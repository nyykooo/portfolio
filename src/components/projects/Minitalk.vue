<template>
    <div>
        <span style="font-size: 24px; color: white;">
            Minitalk is a simple client-server program that allows two processes to communicate with each other using signals. The way my project works is a binary conversion of the signals, as I only used SIGUSR1 and SIGUSR2 each one representing a 0 or a 1. The server is able to receive messages from multiple clients at the same time. For the bonus part my project is able to print unicode chars and emojis, and after printing a message the server sends a signal to the client to confirm that the message was received.
        </span>
    </div>
</template>
